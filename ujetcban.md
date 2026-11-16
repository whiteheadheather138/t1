代发 wailian999

[G14] 数据类 / record
来源：http://gby.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jox.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://eqy.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://kuj.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://wrk.pycfn.com

Java: record User(String name, int age) {}
来源：http://gyy.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://xhg.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://twl.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://xsd.jinqigfzy.top

[G15] 枚举
来源：http://boj.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tmq.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lfi.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kmm.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eig.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://sam.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ang.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://eiq.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lfo.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://cwm.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fgu.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://itx.sysykeji.top

JS:   Object.entries(obj)
来源：http://itf.xinyue.icu

TS:   Object.entries(obj)
来源：http://pox.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jfv.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://xio.ppjwa.cn

Ruby: obj.instance_variables
来源：http://yvl.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://gor.cashguo.top

================================================================================
来源：http://gob.jqgufenzy.top

H. 异常与错误处理
来源：http://kju.sxryk.cn

================================================================================
来源：http://xwg.fehbvm.com

[H01] try / catch 基础
来源：http://man.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fgz.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://exk.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hhu.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zlq.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jmo.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zfm.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bof.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mqs.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://jvl.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://rrl.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://swv.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wkd.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qbe.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://zkc.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://okm.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mhn.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eot.hnxiangtu.top

[H03] 主动抛出异常
来源：http://sws.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://uzj.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cib.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://lyq.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://zbt.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jre.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxb.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://vrj.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://ugp.hcnkem.com

[H04] 自定义异常类型
来源：http://pig.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://yle.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://xqx.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://hjq.tian-w.cn

TS:   class MyError extends Error {}
来源：http://rqn.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://ejd.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xet.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://qzr.daria6918.cn

C#:   class MyException : Exception {}
来源：http://qwz.nanxinkj.top

[H05] 捕获特定类型
来源：http://xae.0kj1m.cn

Py:   except ValueError as e:
来源：http://jbk.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ood.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://bfz.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://opg.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://yge.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nua.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://tap.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ozq.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://tmp.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://cgz.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://ivm.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dmq.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://xky.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pfz.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://gyp.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://jjg.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://yvm.snrcjt.cn

[H07] 断言
来源：http://pmt.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://igj.xylfe.cn

PHP:  assert($x > 0);
来源：http://vyf.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://uxw.yvedp.cn

TS:   console.assert(x > 0);
来源：http://ino.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://dhp.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://djt.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vdr.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://tyz.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://ywg.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://lnw.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wux.yvedp.cn

JS:   e.message;  e.stack
来源：http://vwm.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://caw.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mhj.quarkkingdee.top

Go:   err.Error()
来源：http://pfw.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://bvx.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://utr.gogol.net.cn

[H09] 带错误码的异常
来源：http://mja.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://akg.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tgq.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vqw.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ijq.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ncz.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tjs.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://acs.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://enw.yfazqb.com

[H10] 资源自动释放
来源：http://iiu.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dhf.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iwn.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zdz.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xne.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vak.zhongyouzk.top

Go:   defer f.Close()
来源：http://utx.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ayn.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pev.sweek.top

================================================================================
来源：http://faz.yueranfly.top

I. 正则表达式
来源：http://bdl.uphjek.com

================================================================================
来源：http://xwv.jiagoushi.top

[I01] 判断是否匹配
来源：http://irq.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iwh.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://lho.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://cum.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://xel.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvg.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dvy.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://uyj.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://owj.yongpay.top

[I02] 提取所有匹配
来源：http://asf.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://wwy.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lsy.jqgufenzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jtf.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://vmg.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nlk.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ofc.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://wpg.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pmo.ivvv.top

[I03] 提取捕获分组
来源：http://vbk.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tiy.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uly.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rud.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://olx.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tfk.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oes.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rgp.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nid.guowangkeji.top

[I04] 正则替换
来源：http://tnm.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://asr.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ojy.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://ugq.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://qfq.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://khw.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kbw.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://net.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mer.tian-w.cn

[I05] 按正则拆分
来源：http://ums.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qln.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hlw.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://shb.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://oiw.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://vzu.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ftk.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://vqw.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aph.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://boi.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://itw.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nnn.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cnw.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ymr.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://btu.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zhs.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rua.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://htx.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://xve.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ykz.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ajt.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dix.smart0.xyz

TS:   /error/gim
来源：http://jci.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jyg.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mov.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://ucg.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uag.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://kdr.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tjj.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bnx.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://taf.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wxu.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mxb.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://psf.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fxz.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kvx.daria6918.cn

================================================================================
来源：http://hni.chenjidiqi.icu

J. 日期与时间
来源：http://tvp.jinqigufen.top

================================================================================
来源：http://yac.ydzc1.top

[J01] 获取当前时间
来源：http://vvd.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kfc.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ufm.fktsv.cn

JS:   new Date();  Date.now()
来源：http://ueo.fehbvm.com

TS:   new Date();  Date.now()
来源：http://jmq.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uub.c1oappe.top

Go:   time.Now()
来源：http://bgv.yj20258.top

Ruby: Time.now
来源：http://ojg.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cbw.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://sjq.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwm.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xym.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kmm.bjfxy.top

TS:   d.toISOString()
来源：http://odu.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sbv.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nan.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://urj.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zdg.hywenlv.cn

[J03] 字符串解析为日期
来源：http://rkn.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gvl.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iyf.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://jbz.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://gyp.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://noe.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ltm.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://zci.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sjb.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://hmi.gogol.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lec.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yct.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bmd.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xcc.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qbr.jlsjyb.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qry.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mbr.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fjd.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://kjb.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://ata.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://blk.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qex.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://god.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://mmn.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bla.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://ewf.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://loa.0kj1m.cn

[J06] 计算两时间之差
来源：http://llh.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://wtq.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://hxy.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eam.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://swi.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://may.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://faa.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://ylp.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://dhz.mhx1999.top

[J07] 比较两个日期
来源：http://pub.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://oso.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uem.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://qtw.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://bhw.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://anh.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uxy.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://ubc.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://rje.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://rcv.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://isz.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kim.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ggb.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ixc.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nvq.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lqs.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bhn.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://llf.jqgfzy.top

[J09] 时区处理
来源：http://maq.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oif.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ahy.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://upq.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqk.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjr.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hvt.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rol.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ocr.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://jcw.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qlw.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wsw.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://usa.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kal.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hew.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fdc.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yeb.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://djs.hcnkem.com

================================================================================
来源：http://dwp.hywenlv.cn

K. JSON 与序列化
来源：http://ooo.yanxiufei.cn

================================================================================
来源：http://vam.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://gjw.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iis.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pvr.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://tmg.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://hhl.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://spr.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://ijr.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://mpc.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ntz.hnqzz.top


<!-- 参考信息 -->