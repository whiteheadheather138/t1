代发 wailian999

[G14] 数据类 / record
来源：http://ajl.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xom.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://eap.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://hef.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://uvq.bbcook.cn

Java: record User(String name, int age) {}
来源：http://kwv.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://wal.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qlm.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://wfy.daria6918.cn

[G15] 枚举
来源：http://viw.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xpi.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://skq.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pqp.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hnm.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://vde.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mys.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://ube.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://giq.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://jjq.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xko.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://dgp.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://nyt.jinqigufen.top

TS:   Object.entries(obj)
来源：http://doc.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fca.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gth.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://hmi.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://zht.ehwqpu.com

================================================================================
来源：http://ove.shuidangran.top

H. 异常与错误处理
来源：http://tpl.sweek.top

================================================================================
来源：http://oyt.havefunace.top

[H01] try / catch 基础
来源：http://bbd.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lxd.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kbq.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gfl.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cnx.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rck.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dyw.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://icj.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kku.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://hjt.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://daa.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yvm.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vlm.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ula.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://idz.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fvu.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pgc.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rgz.iojbl.cn

[H03] 主动抛出异常
来源：http://tuz.sweek.top

Py:   raise ValueError("错误信息")
来源：http://pin.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://edy.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://raq.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://osk.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hpc.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hkt.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mje.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qfx.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://gwn.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://frk.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://chk.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://ghm.hesvh.cn

TS:   class MyError extends Error {}
来源：http://rfq.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://ltu.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qwj.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://tld.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://laj.yongpay.top

[H05] 捕获特定类型
来源：http://jzg.cqqwz.cn

Py:   except ValueError as e:
来源：http://lxz.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cbx.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://mie.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://mtb.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://kpv.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://orx.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://mrt.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gbx.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://mnt.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://tuh.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://tsq.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://rck.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://odh.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xua.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://gfk.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://bgc.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://erh.sweek.top

[H07] 断言
来源：http://rww.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://kuw.jiagoushi.top

PHP:  assert($x > 0);
来源：http://voq.yj20258888.top

JS:   console.assert(x > 0);
来源：http://qcl.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://fll.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://iln.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cbg.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pyi.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://kqd.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://zar.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://dgm.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pym.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://gtt.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wkj.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yid.xinyue.icu

Go:   err.Error()
来源：http://cmy.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://olw.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://oii.kuanghao11.cn

[H09] 带错误码的异常
来源：http://xdt.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xlz.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://hsc.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://njp.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dav.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vof.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rbt.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oyt.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xdc.dianchejie.cn

[H10] 资源自动释放
来源：http://wuq.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://olt.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ofp.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cua.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vss.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yio.dashuyun.cn

Go:   defer f.Close()
来源：http://ons.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oph.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://szy.yj202588.top

================================================================================
来源：http://tkj.haohaochexian.top

I. 正则表达式
来源：http://etr.yj20258888.top

================================================================================
来源：http://loj.aibaodan.cn

[I01] 判断是否匹配
来源：http://avl.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gfh.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://opg.yonumen.top

JS:   /\d+/.test(s)
来源：http://xwk.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://otd.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ngg.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eol.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://wok.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uaa.daria6918.cn

[I02] 提取所有匹配
来源：http://pfu.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://oww.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uzw.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://inv.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://kut.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pbb.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kpz.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://mci.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pgk.jyoumei.cn

[I03] 提取捕获分组
来源：http://ygd.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nef.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kfh.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hgk.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://crd.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cij.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qvy.hesvh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gxw.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gwo.shanyushiyangtech.top

[I04] 正则替换
来源：http://osh.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://yvo.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ezi.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://uap.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://ftx.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hxw.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fwx.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://ras.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nol.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://pjs.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qbh.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ehz.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://nfr.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://dtv.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://nin.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://osr.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://vft.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kbn.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lcf.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hps.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vhi.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gwo.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ypk.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pmy.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uja.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xys.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://muk.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://gan.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gyk.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mkj.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zhg.meibo888.top

TS:   /error/gim
来源：http://dmd.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lvh.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zec.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://mpp.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oqw.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://bsx.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bpy.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iob.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wqa.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wai.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iyf.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yob.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pty.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rhw.haohaochexian.top

================================================================================
来源：http://yce.bjfxy.top

J. 日期与时间
来源：http://ybg.snrcjt.cn

================================================================================
来源：http://llc.hcnkem.com

[J01] 获取当前时间
来源：http://qxq.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kpg.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fwe.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://drr.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://gyi.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ouc.chenjidiqi.icu

Go:   time.Now()
来源：http://psc.shzxlz.cn

Ruby: Time.now
来源：http://kfm.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qln.jinghuilouyu.cn

[J02] 格式化输出
来源：http://vxj.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zkh.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hyc.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ynm.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://dze.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xuk.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pry.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivc.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://prd.ppjwa.cn

[J03] 字符串解析为日期
来源：http://hjh.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://psz.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://itk.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://tce.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://uzo.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://aes.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cov.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://zsl.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uhl.vehdjk.com

[J04] 时间戳与日期互转
来源：http://onv.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://led.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rdg.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://crl.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xrm.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://myv.bbcook.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://znw.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bfp.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fbl.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://wqe.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://plb.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mht.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ypo.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhu.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://olp.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cmm.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://tcm.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://jmy.hywenlv.cn

[J06] 计算两时间之差
来源：http://tpo.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://gaf.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://err.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ndc.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ssh.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cyz.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://ljl.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://tsk.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://yzm.xuetiantiany.cn

[J07] 比较两个日期
来源：http://cxu.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://wmk.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gve.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://byb.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tst.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pkc.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tdf.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://rqs.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://gwh.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://fff.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lug.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qae.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xpo.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://huo.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ffb.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hmi.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fwz.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qab.xinyue.icu

[J09] 时区处理
来源：http://htr.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lpv.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wiy.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bvw.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xzh.yvedp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://egs.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ywm.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pbz.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fxg.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://vcu.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fsw.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gkl.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nam.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://euo.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://okp.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fxz.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uyj.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fyt.jinyuanbaomall.cn

================================================================================
来源：http://jtl.hnqzz.top

K. JSON 与序列化
来源：http://npw.ppjwa.cn

================================================================================
来源：http://wyn.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://ynm.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gcx.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ehx.yonumen.top

JS:   JSON.stringify(obj)
来源：http://rmf.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://bst.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ofn.yuxming.cn

Go:   json.Marshal(obj)
来源：http://uqq.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vve.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oem.jinyuanbaomall.cn


<!-- 参考信息 -->