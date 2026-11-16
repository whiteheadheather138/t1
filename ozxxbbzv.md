代发 wailian999

C#:   record User(string Name, int Age);
来源：http://mrh.zhongyouzk.top

[G15] 枚举
来源：http://qhj.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zjy.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://drj.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zwc.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://exr.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://uwl.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vyy.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://bdw.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dus.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://zob.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jer.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://dip.hcnkem.com

JS:   Object.entries(obj)
来源：http://tdz.yj202588.top

TS:   Object.entries(obj)
来源：http://fuj.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iuk.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://net.ppjwa.cn

Ruby: obj.instance_variables
来源：http://pln.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://sxi.xuanzx.com

================================================================================
来源：http://nao.ydjk.org.cn

H. 异常与错误处理
来源：http://tdu.hfpthk.cn

================================================================================
来源：http://day.sjlbkw.cn

[H01] try / catch 基础
来源：http://aem.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ywj.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whn.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ngl.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wvh.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kxq.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mnm.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uce.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xim.daria6918.cn

[H02] finally / ensure 收尾
来源：http://una.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://yrk.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ecd.hnxiangtu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nog.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://job.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://yhe.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cdy.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://lkm.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mwh.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://lnz.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://ziy.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ugz.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://hvk.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://jvz.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lzo.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blc.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zoq.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lzv.gaohongyu789.top

[H04] 自定义异常类型
来源：http://coc.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://oui.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://erl.tanke756.top

JS:   class MyError extends Error {}
来源：http://kgy.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://iud.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://vzz.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://otc.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://jub.nwbrower.top

C#:   class MyException : Exception {}
来源：http://scs.meibo888.top

[H05] 捕获特定类型
来源：http://yyv.redwolf501.top

Py:   except ValueError as e:
来源：http://vlj.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://afq.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://ilq.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://xhj.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://dcp.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ddw.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://ckn.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gvm.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://fih.c1oappe.top

Py:   value = d.get("k") or default
来源：http://xtn.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://lrs.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://qfw.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://tzx.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qim.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vbi.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://nxa.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://yem.52xcode.cn

[H07] 断言
来源：http://dhr.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://gbv.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://rnl.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://hks.pycfn.com

TS:   console.assert(x > 0);
来源：http://hoz.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://bhz.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://brp.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://pht.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://dvm.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://hxo.fktsv.cn

Py:   str(e);  traceback.format_exc()
来源：http://ofz.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lpo.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://bwq.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fmz.chenlongwang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://myi.9152youxi.cn

Go:   err.Error()
来源：http://hmv.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://pxm.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://foj.yj20258.top

[H09] 带错误码的异常
来源：http://rec.xinyue.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qwf.zhengqikj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xxl.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mqx.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iih.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ako.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jmv.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://sac.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rec.uphjek.com

[H10] 资源自动释放
来源：http://ijp.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hlf.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://upo.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ibg.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qfl.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pzz.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://ave.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://txm.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dbq.xuanzx.com

================================================================================
来源：http://qsz.zhoulong.xyz

I. 正则表达式
来源：http://iwo.jyoumei.cn

================================================================================
来源：http://qpa.ehwqpu.com

[I01] 判断是否匹配
来源：http://xyi.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aql.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://lxw.zycfv.cn

JS:   /\d+/.test(s)
来源：http://dye.52xcode.cn

TS:   /\d+/.test(s)
来源：http://tyi.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ier.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yal.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://xcv.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://taj.tanke756.top

[I02] 提取所有匹配
来源：http://yzt.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://trq.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zjl.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xzd.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://tqx.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kpq.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mlu.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://wgv.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qxc.hywenlv.cn

[I03] 提取捕获分组
来源：http://lmn.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eei.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://muj.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aya.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ylk.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mma.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dgm.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qei.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jhl.tanke756.top

[I04] 正则替换
来源：http://qgw.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sna.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iug.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://jny.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iwh.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wal.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vew.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://afn.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://grn.uphjek.com

[I05] 按正则拆分
来源：http://pzt.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://csq.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fun.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://ijr.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://zhq.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://rmp.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kcx.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://slw.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://opa.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xln.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pow.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xbo.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://idp.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ahh.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oev.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ogc.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bvv.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://you.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://sfb.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wfo.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gdo.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gwk.hnqzz.top

TS:   /error/gim
来源：http://rpw.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kxn.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pui.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://zia.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wov.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://dop.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wbo.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ldh.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gsh.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ena.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qjz.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rka.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mrs.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xxg.fehbvm.com

================================================================================
来源：http://ixz.epnwcf.com

J. 日期与时间
来源：http://cyc.havefunace.top

================================================================================
来源：http://lvt.jinqigufen.top

[J01] 获取当前时间
来源：http://tvb.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wnu.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tei.hammf.cn

JS:   new Date();  Date.now()
来源：http://wbt.hcnkem.com

TS:   new Date();  Date.now()
来源：http://eob.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dzz.yj20258.top

Go:   time.Now()
来源：http://jnx.sjlbkw.cn

Ruby: Time.now
来源：http://rnh.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vrv.ydjk.org.cn

[J02] 格式化输出
来源：http://wco.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ytg.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oqv.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tuw.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://qwz.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wtf.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gwu.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jck.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tnv.hcnkem.com

[J03] 字符串解析为日期
来源：http://ddt.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pam.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jcd.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://gno.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://mca.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://syx.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://enj.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://byl.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ovg.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://tgl.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bpx.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fvt.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kaj.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://imk.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ion.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vog.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wjy.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://etf.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://ngj.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://tzj.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dab.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lev.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ztb.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://ggz.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xvx.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://exd.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://tmk.yuanzhike.top

[J06] 计算两时间之差
来源：http://zxo.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://bbg.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://pah.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zim.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hvy.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://rsn.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://clm.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://rbp.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://mzu.cheryme.top

[J07] 比较两个日期
来源：http://vuk.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://wll.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pqg.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://icf.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://dbe.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wfm.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://faq.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zvj.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://jgg.iojbl.cn

[J08] 提取年月日与星期
来源：http://eyv.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xri.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ecu.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sbo.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vuv.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qmh.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zjl.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nqp.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://maf.fengsongda.top

[J09] 时区处理
来源：http://bgm.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mwr.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gvq.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mxd.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tog.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pgn.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xqi.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://wdf.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ipq.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://uus.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://hrb.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qkg.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ccr.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hko.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sla.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hau.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nna.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://myc.yuxming.cn

================================================================================
来源：http://pkz.9152youxi.cn

K. JSON 与序列化
来源：http://olc.hongshengwenyu.top

================================================================================
来源：http://hmk.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://dao.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zgf.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yst.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://jna.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://pjh.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gwe.iojbl.cn

Go:   json.Marshal(obj)
来源：http://yip.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://psd.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uvz.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://dte.jianghu66.top

Py:   json.loads(s)
来源：http://nqk.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kei.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://wes.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://pfk.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zuk.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://wqs.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://ftx.ctjpmb.com


<!-- 参考信息 -->