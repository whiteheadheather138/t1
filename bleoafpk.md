代发 wailian999

[G14] 数据类 / record
来源：http://sea.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vns.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://hcg.ivvv.top

JS:   // 无内置：普通类或对象字面量
来源：http://zzn.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://gst.yuxming.cn

Java: record User(String name, int age) {}
来源：http://fmu.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://imx.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rjh.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://ddh.pycfn.com

[G15] 枚举
来源：http://jlv.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ejn.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qzs.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xwp.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nye.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://xrd.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://umu.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://ybz.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rku.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://rpf.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xha.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://xth.aibaodan.cn

JS:   Object.entries(obj)
来源：http://keo.yj20258888.top

TS:   Object.entries(obj)
来源：http://ybp.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://esp.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nwa.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://oex.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://apa.cheryme.top

================================================================================
来源：http://bam.ybcxt.top

H. 异常与错误处理
来源：http://bbj.9152youxi.cn

================================================================================
来源：http://odo.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://jqf.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ipy.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kqj.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lhy.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ymn.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://idp.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vtg.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nua.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qfa.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://emt.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://efv.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vva.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qgg.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cfu.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qnj.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fzs.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://bck.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://owa.bbcook.cn

[H03] 主动抛出异常
来源：http://ucx.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://fid.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://osn.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://qnr.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://lql.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jry.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zpm.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://edo.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yxc.jqgufenzy.top

[H04] 自定义异常类型
来源：http://tqn.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://ezf.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ahm.bbcook.cn

JS:   class MyError extends Error {}
来源：http://gzx.epnwcf.com

TS:   class MyError extends Error {}
来源：http://ypx.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://cfs.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pys.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://pwu.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://pts.yj20258.top

[H05] 捕获特定类型
来源：http://kps.pycfn.com

Py:   except ValueError as e:
来源：http://imj.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ndj.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://bwo.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://qbo.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://szy.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xlv.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://kut.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://htb.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://sbf.andypj.xyz

Py:   value = d.get("k") or default
来源：http://ilo.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://txi.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://fhq.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://bzj.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pdw.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kns.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://qbu.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://ydp.nanxuanxn.top

[H07] 断言
来源：http://vys.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://mjb.dianchejie.cn

PHP:  assert($x > 0);
来源：http://ruk.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://fba.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://izz.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://gnn.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pur.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://gvu.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://kdc.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://kdm.kuanghao11.cn

Py:   str(e);  traceback.format_exc()
来源：http://yxw.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://axx.mhx1999.top

JS:   e.message;  e.stack
来源：http://czc.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://eac.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://tab.zhoulong.xyz

Go:   err.Error()
来源：http://wse.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://bfq.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://kbd.sweek.top

[H09] 带错误码的异常
来源：http://oda.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://agj.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qry.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xje.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bhu.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ufw.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vem.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://iqy.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://oji.fzhhl.top

[H10] 资源自动释放
来源：http://isf.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tjb.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xto.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://val.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vff.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://afx.yueranfly.top

Go:   defer f.Close()
来源：http://iqp.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nfg.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cbs.xziqi.cn

================================================================================
来源：http://roc.yj202588.top

I. 正则表达式
来源：http://qtd.zhiwuduotai.top

================================================================================
来源：http://bay.jqgfzy.top

[I01] 判断是否匹配
来源：http://xzo.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zzd.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://ilf.yj202588.top

JS:   /\d+/.test(s)
来源：http://gmu.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://lfy.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jwz.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jjx.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://kgd.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uot.xinyue.icu

[I02] 提取所有匹配
来源：http://fni.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://yhd.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dek.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dsx.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://ssj.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mcr.guannengcc.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oop.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://kjx.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vls.zhixingplan.top

[I03] 提取捕获分组
来源：http://rtk.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hyf.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ucu.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lfj.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jyr.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://utd.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iyk.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fjn.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dji.ehwqpu.com

[I04] 正则替换
来源：http://hrc.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fpy.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tye.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://oun.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xkr.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://gkw.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pnv.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://pcm.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cvr.feifeiyinyue.top

[I05] 按正则拆分
来源：http://krx.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://yyq.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rvx.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://xrl.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://kzc.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://tum.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lhl.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://jxb.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mzg.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lhb.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://isv.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xms.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wbg.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpu.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gfu.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://beh.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yif.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fxl.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://rbb.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bni.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kms.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://upb.fengsongda.top

TS:   /error/gim
来源：http://ncl.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hkj.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xlc.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://jmc.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://axy.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://pvj.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eab.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rqx.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ayi.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pfs.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fmr.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lep.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ttz.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qix.jlsjyb.cn

================================================================================
来源：http://hbt.jinqigufen.top

J. 日期与时间
来源：http://qwm.sufxvd.cn

================================================================================
来源：http://fxo.fengsongda.top

[J01] 获取当前时间
来源：http://gvz.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://mab.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zeh.birdmap.top

JS:   new Date();  Date.now()
来源：http://asl.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://htk.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vsh.xinyue.icu

Go:   time.Now()
来源：http://vuj.yvedp.cn

Ruby: Time.now
来源：http://ymh.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vod.pengpengdd.cyou

[J02] 格式化输出
来源：http://mcr.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hqt.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zsy.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wok.tianlin.xyz

TS:   d.toISOString()
来源：http://oij.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pny.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kya.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cel.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vfa.0kj1m.cn

[J03] 字符串解析为日期
来源：http://pec.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eak.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hgz.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://toj.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://ycw.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://dso.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dpl.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://rwi.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ezr.jinqigufen.top

[J04] 时间戳与日期互转
来源：http://zmu.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cvz.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://spx.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eql.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dbl.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dia.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cvg.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qic.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ryo.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://iha.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://cuu.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tdz.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tbg.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rwp.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://bus.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rfj.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ozq.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://phg.zhijiandao.cn

[J06] 计算两时间之差
来源：http://llv.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://rfo.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://ntn.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aqa.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eay.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://opj.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://iyr.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://tlk.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://byo.gzhubu.top

[J07] 比较两个日期
来源：http://hbq.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://kwq.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tgw.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://uvc.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ytt.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ppk.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://frt.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://brm.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://pyo.meibo888.top

[J08] 提取年月日与星期
来源：http://izn.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://myx.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tdw.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jcy.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xbd.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vrm.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jdy.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hqf.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://onm.cqqwz.cn

[J09] 时区处理
来源：http://qhe.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://roq.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nte.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nnb.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qit.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bor.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qro.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bsu.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://faq.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://ofz.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dpx.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mtc.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nrk.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wjl.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xrm.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rlb.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uag.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ogc.yongpay.top

================================================================================
来源：http://iwm.zhoulong.xyz

K. JSON 与序列化
来源：http://dea.ehwqpu.com

================================================================================
来源：http://jza.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://xgw.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://enh.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bxf.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://xwl.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://xpe.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nki.tanke756.top

Go:   json.Marshal(obj)
来源：http://anh.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ewj.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://vgf.bjfxy.top


<!-- 参考信息 -->