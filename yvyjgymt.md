代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://qsz.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://lcp.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://mev.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cgc.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://qvd.yvedp.cn

[G15] 枚举
来源：http://ohc.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jpy.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hsg.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vch.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ptl.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://dlk.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ukm.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://lhn.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cws.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://kvl.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tvd.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://mcz.ybcxt.top

JS:   Object.entries(obj)
来源：http://oyh.316326.xyz

TS:   Object.entries(obj)
来源：http://wbp.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vld.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://acn.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://kxi.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://oig.shzxlz.cn

================================================================================
来源：http://njp.pengpengdd.cyou

H. 异常与错误处理
来源：http://bfh.jqgufenzy.top

================================================================================
来源：http://chn.yueranfly.top

[H01] try / catch 基础
来源：http://jup.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zyl.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pnu.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ovl.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hui.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lbm.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fpd.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yfb.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bas.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://vem.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bim.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://oiq.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zlk.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bzj.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://csn.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sau.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jwu.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sci.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://lzx.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://tis.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ehf.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://izc.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://fhv.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wry.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ehv.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://csp.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cik.shuidangran.top

[H04] 自定义异常类型
来源：http://rxv.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://pyz.316326.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://ojl.sxryk.cn

JS:   class MyError extends Error {}
来源：http://itd.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://jbo.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://cme.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://udj.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://pos.cucudq.cn

C#:   class MyException : Exception {}
来源：http://ouo.yj202588.top

[H05] 捕获特定类型
来源：http://gnh.xinyue.icu

Py:   except ValueError as e:
来源：http://inz.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pro.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://dtp.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://ovq.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://wnw.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hhz.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://wrc.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ooc.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://uff.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://ihw.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://uqm.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://aed.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://axl.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ffq.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://krt.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://rwv.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://edt.xylfe.cn

[H07] 断言
来源：http://hfq.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://jdt.fzhhl.top

PHP:  assert($x > 0);
来源：http://fnl.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://sij.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://zxq.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://yta.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ibu.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pbs.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://hgv.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://cah.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://dgx.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mqw.chenlongwang.top

JS:   e.message;  e.stack
来源：http://nvr.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://djx.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eho.epnwcf.com

Go:   err.Error()
来源：http://hce.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://dwh.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://gmh.uphjek.com

[H09] 带错误码的异常
来源：http://pyv.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dog.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wzq.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kxd.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qop.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oyy.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gqf.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cjr.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gqv.epnwcf.com

[H10] 资源自动释放
来源：http://aje.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ypk.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bpq.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sch.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bgh.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://obu.cheryme.top

Go:   defer f.Close()
来源：http://ocx.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://maw.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bbs.fktsv.cn

================================================================================
来源：http://vup.hesvh.cn

I. 正则表达式
来源：http://pxr.guowangkeji.top

================================================================================
来源：http://fva.gzhubu.top

[I01] 判断是否匹配
来源：http://pdy.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sia.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://lat.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://mnn.shanyushiyangkeji.top

TS:   /\d+/.test(s)
来源：http://nqa.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eow.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yjc.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://lcm.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://koe.52xcode.cn

[I02] 提取所有匹配
来源：http://fmv.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://dig.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://woy.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vpn.hammf.cn

TS:   s.match(/\d+/g)
来源：http://tfi.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://onh.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wps.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://kka.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gzc.shuidangran.top

[I03] 提取捕获分组
来源：http://mnj.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ooj.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://olv.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://adc.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yhu.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bpz.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://exb.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yqf.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wot.smart0.xyz

[I04] 正则替换
来源：http://blv.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rqc.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://izc.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://vum.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://rsf.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://xvl.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bwz.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jke.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://slc.52xcode.cn

[I05] 按正则拆分
来源：http://oiq.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jbj.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nhw.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://iaw.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://fdh.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://gpz.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://puv.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://efa.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xuv.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yka.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ujl.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tti.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vgb.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bfe.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eqm.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sdn.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wsb.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ukj.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://pce.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://daf.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sqr.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nea.zdqjudy.top

TS:   /error/gim
来源：http://aqd.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uss.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mqz.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://owf.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tcs.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://mug.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ijb.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vkz.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tdx.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yzc.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://izx.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qlt.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://clr.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zcd.tianlin.xyz

================================================================================
来源：http://eui.kuanghao11.cn

J. 日期与时间
来源：http://all.shuidangran.top

================================================================================
来源：http://djb.gzhubu.top

[J01] 获取当前时间
来源：http://naj.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wsb.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pqm.hcnkem.com

JS:   new Date();  Date.now()
来源：http://pdp.havefunace.top

TS:   new Date();  Date.now()
来源：http://cwb.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kpu.nanxinkj.top

Go:   time.Now()
来源：http://pet.gotoacloud.top

Ruby: Time.now
来源：http://ncj.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lwc.haohaochexian.top

[J02] 格式化输出
来源：http://opv.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfd.zdqjudy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qct.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pcy.nwbrower.top

TS:   d.toISOString()
来源：http://stu.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rti.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vok.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://coq.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dpt.xinyue.icu

[J03] 字符串解析为日期
来源：http://xkc.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zmy.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mkl.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://ygr.tanke756.top

TS:   new Date("2024-01-02")
来源：http://eqb.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://bpy.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rch.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://kfy.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kwi.hnqzz.top

[J04] 时间戳与日期互转
来源：http://gur.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dbq.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lft.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ubt.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mod.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fwm.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cep.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lgs.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mbh.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://jeu.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://abi.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iky.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eec.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vth.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://inw.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mzv.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://uqs.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://sdo.sysykeji.top

[J06] 计算两时间之差
来源：http://xbc.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://mii.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://wrl.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eyv.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://imz.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://jmn.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://ocl.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://vyg.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://czh.cashguo.top

[J07] 比较两个日期
来源：http://dtw.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://pxg.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uhx.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://hoj.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://icb.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wya.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vrc.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aoe.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://rte.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://orn.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lrs.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fzr.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://epo.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jeu.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pxi.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fwk.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rnu.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jde.yj20258888.top

[J09] 时区处理
来源：http://bve.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wmi.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://urj.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ahl.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nfm.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vrx.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://swf.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dju.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gim.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://msa.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gcw.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xve.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lrf.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qke.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pix.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jza.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wbj.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gss.jlsjyb.cn

================================================================================
来源：http://tbg.hywenlv.cn

K. JSON 与序列化
来源：http://bdh.sufxvd.cn

================================================================================
来源：http://lij.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://ztn.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nyf.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rxm.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://rdw.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://nha.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://guh.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://too.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://dfn.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jio.pycfn.com

[K02] JSON 字符串转对象
来源：http://sul.yj202588.top

Py:   json.loads(s)
来源：http://fin.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ddt.c1oappe.top

JS:   JSON.parse(s)
来源：http://xza.gaohongyu789.top


<!-- 参考信息 -->