代发 wailian999

Java: u instanceof User
来源：http://jax.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wvb.ybcxt.top

Ruby: u.is_a?(User)
来源：http://prs.snrcjt.cn

C#:   u is User
来源：http://vjy.cashguo.top

[G14] 数据类 / record
来源：http://nez.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oiq.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://xxb.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mmy.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://pjf.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://bbr.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://hle.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhc.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://ltf.vqdsnc.cn

[G15] 枚举
来源：http://drb.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ayx.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wnf.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zmx.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rtl.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://ghu.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://izd.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://ibx.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kum.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://arm.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pbx.yonumen.top

PHP:  get_object_vars($obj);
来源：http://enm.cdnleiting.top

JS:   Object.entries(obj)
来源：http://des.daxiang520.top

TS:   Object.entries(obj)
来源：http://jjs.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ltk.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jnu.9152youxi.cn

Ruby: obj.instance_variables
来源：http://qnr.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://cvi.zdbjq.cn

================================================================================
来源：http://qze.tianlin.xyz

H. 异常与错误处理
来源：http://vmp.uphjek.com

================================================================================
来源：http://rkb.smart0.xyz

[H01] try / catch 基础
来源：http://eih.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aue.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yol.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qzg.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dip.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fxq.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uze.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jmq.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ehp.hnqzz.top

[H02] finally / ensure 收尾
来源：http://isk.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://uur.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oyl.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ykc.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uxn.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://peq.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ouk.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rcv.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tjq.cheryme.top

[H03] 主动抛出异常
来源：http://ihp.sweek.top

Py:   raise ValueError("错误信息")
来源：http://mjz.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zni.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://nyt.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://xjd.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qno.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hgy.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sci.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cgg.yanxiufei.cn

[H04] 自定义异常类型
来源：http://xpe.havefunace.top

Py:   class MyError(Exception): pass
来源：http://jcc.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ytb.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://bsi.havefunace.top

TS:   class MyError extends Error {}
来源：http://iuh.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://mru.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://npk.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://ebe.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://kin.mhx1999.top

[H05] 捕获特定类型
来源：http://lpi.daxiang520.top

Py:   except ValueError as e:
来源：http://acx.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yab.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://zaz.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://bkf.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://rnh.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ogn.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://jgx.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://och.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://cex.xylfe.cn

Py:   value = d.get("k") or default
来源：http://awo.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vyz.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://zjh.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://hfp.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jgv.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://biy.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://kur.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://dcw.yuxming.cn

[H07] 断言
来源：http://bui.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://iwj.jinghuilouyu.cn

PHP:  assert($x > 0);
来源：http://ppe.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://hgf.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://zdd.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://civ.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sag.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://myf.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://zti.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://mjk.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://piy.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yir.yangfankeji.com

JS:   e.message;  e.stack
来源：http://uws.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://knx.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iqo.chenzaomai.com

Go:   err.Error()
来源：http://wlj.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://vgh.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://xzm.shzxlz.cn

[H09] 带错误码的异常
来源：http://alb.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rfy.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://exy.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wqv.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ntk.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uzg.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://liq.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gqm.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hkn.yj20258888.top

[H10] 资源自动释放
来源：http://bkl.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mwz.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qgx.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dex.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jgt.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://whl.zhixingplan.top

Go:   defer f.Close()
来源：http://vsg.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pkh.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ktn.xziqi.cn

================================================================================
来源：http://hcg.birdmap.top

I. 正则表达式
来源：http://ywt.aizwys.cn

================================================================================
来源：http://dky.gotoacloud.top

[I01] 判断是否匹配
来源：http://bpa.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fjz.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://rus.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://vxv.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://hpl.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ldb.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqi.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://upg.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rxr.guowangkeji.top

[I02] 提取所有匹配
来源：http://euc.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://pkj.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vgi.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://boj.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://agg.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://htf.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dnt.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://hsm.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pqt.yonumen.top

[I03] 提取捕获分组
来源：http://rfg.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ylg.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ouy.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dhi.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cmi.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lqp.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://poj.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oez.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qko.redwolf501.top

[I04] 正则替换
来源：http://ylo.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hgn.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://luc.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ohm.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://qqm.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kce.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hco.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://afq.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mfb.yuanzhike.top

[I05] 按正则拆分
来源：http://anl.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rxb.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://flh.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://lyd.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://nwa.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://zdw.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://azo.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tjm.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qzp.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qtf.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://elr.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sjw.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xdy.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gjv.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kdv.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jkz.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xky.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://acu.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://jwv.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ajz.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vrx.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zzb.dashuyun.cn

TS:   /error/gim
来源：http://gqo.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://djc.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bso.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://tga.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iil.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://itw.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oba.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://amk.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oqo.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qjq.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rms.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nxg.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xku.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kdl.0kj1m.cn

================================================================================
来源：http://dnk.yuxming.cn

J. 日期与时间
来源：http://kwr.jiagoushi.top

================================================================================
来源：http://zai.ctjpmb.com

[J01] 获取当前时间
来源：http://jqs.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ybs.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hmi.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://ham.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://gen.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jpk.316326.xyz

Go:   time.Now()
来源：http://bxs.yangfankeji.com

Ruby: Time.now
来源：http://gmr.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eas.ybcxt.top

[J02] 格式化输出
来源：http://sfk.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gum.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wfx.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ola.gogol.net.cn

TS:   d.toISOString()
来源：http://vwc.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gio.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tzz.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwu.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kvz.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://vts.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gid.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eay.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://kss.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://xqr.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mcs.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fcd.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://ppb.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hqc.redwolf501.top

[J04] 时间戳与日期互转
来源：http://bya.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://znm.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://liq.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vzh.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mxt.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://igs.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vce.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uwv.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zfe.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://fek.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://scq.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://myb.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqa.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mop.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://gyh.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cxt.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://nli.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kdw.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://nth.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://oaw.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://ppk.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rgo.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oez.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iei.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://ttc.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://dup.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://vxv.feifeiyinyue.top

[J07] 比较两个日期
来源：http://adk.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://fbn.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bsi.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://uvp.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://ksi.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://isf.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ixc.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://osi.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://tci.aizwys.cn

[J08] 提取年月日与星期
来源：http://rmi.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xjy.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oqz.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qjq.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dxl.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lng.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bed.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://izz.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mar.ybcxt.top

[J09] 时区处理
来源：http://ynj.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oth.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ppo.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zcf.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cre.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xgj.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://guq.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bgr.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yus.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://kck.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lks.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fjg.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dwu.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dmx.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pew.yonumen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uya.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gcb.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lnf.shanyushiyangkeji.top

================================================================================
来源：http://zno.fanxiaobao.xyz

K. JSON 与序列化
来源：http://tlz.ppjwa.cn

================================================================================
来源：http://pii.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://ayk.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lzs.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qhc.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://lez.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://tpi.yj20258.top


<!-- 参考信息 -->