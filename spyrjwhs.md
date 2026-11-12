代发 wailian999

Java: u instanceof User
来源：http://cge.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oeg.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://qje.mhx1999.top

C#:   u is User
来源：http://xco.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://nem.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://chf.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://vos.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://wit.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://umw.iojbl.cn

Java: record User(String name, int age) {}
来源：http://ccz.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://jsr.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fnt.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://pra.jyoumei.cn

[G15] 枚举
来源：http://ppk.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nkn.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://alk.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mke.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sse.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://agb.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://edb.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://qif.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vlv.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://qla.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://udb.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://upy.yvedp.cn

JS:   Object.entries(obj)
来源：http://fkr.jqgfzy.top

TS:   Object.entries(obj)
来源：http://kqb.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mtt.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cwl.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://oih.jqgufenzy.top

C#:   // 用反射或 System.Text.Json
来源：http://klh.hfpthk.cn

================================================================================
来源：http://nrc.birdmap.top

H. 异常与错误处理
来源：http://vjq.jyoumei.cn

================================================================================
来源：http://zaw.xylfe.cn

[H01] try / catch 基础
来源：http://rpn.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cff.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kqm.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://soc.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eyk.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vrr.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kaz.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nse.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://atf.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://mko.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://wre.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yuj.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hmm.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sor.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nhe.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xju.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nqn.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://icf.guannengcc.top

[H03] 主动抛出异常
来源：http://uky.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://zxa.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eoo.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://wyr.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://hie.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uxu.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://msu.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qjv.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://dcs.yueranfly.top

[H04] 自定义异常类型
来源：http://iuh.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://lrj.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://ryb.nwbrower.top

JS:   class MyError extends Error {}
来源：http://kfr.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://ugg.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://qsc.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kbq.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://vpx.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://ivv.gogol.net.cn

[H05] 捕获特定类型
来源：http://nbl.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://wbd.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bhx.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://yly.wangshuangyany.cn

TS:   if (e instanceof TypeError) {}
来源：http://bpq.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://avs.jinqigufen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pqb.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://wef.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tbd.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://fxb.hnqzz.top

Py:   value = d.get("k") or default
来源：http://uqk.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://wbt.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bwc.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://kjs.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://afc.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qye.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://ftf.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://wof.ivvv.top

[H07] 断言
来源：http://ibw.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://gtk.fktsv.cn

PHP:  assert($x > 0);
来源：http://kjr.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://jqc.shuidangran.top

TS:   console.assert(x > 0);
来源：http://jbf.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://toa.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jmw.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://fmz.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://sks.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://ofb.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://xce.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tih.ybcxt.top

JS:   e.message;  e.stack
来源：http://myw.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://icz.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ymv.wangshuangyany.cn

Go:   err.Error()
来源：http://zby.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://wnq.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://izv.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://mtg.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gfb.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jui.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oit.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nig.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oli.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qxo.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://wic.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sfd.snrcjt.cn

[H10] 资源自动释放
来源：http://yij.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sam.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hvk.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sju.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iiq.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mcb.hywenlv.cn

Go:   defer f.Close()
来源：http://aca.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://upb.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yrc.ybcxt.top

================================================================================
来源：http://gdp.pengpengdd.cyou

I. 正则表达式
来源：http://haa.hnxiangtu.top

================================================================================
来源：http://zcb.tarul.cn

[I01] 判断是否匹配
来源：http://lfz.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nyi.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://zsq.sysykeji.top

JS:   /\d+/.test(s)
来源：http://vyh.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://kgl.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cjq.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cnr.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://fip.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rst.yueranfly.top

[I02] 提取所有匹配
来源：http://sfd.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://vut.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yig.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://htf.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://jle.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mwn.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rxl.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://vgl.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wqz.bjfxy.top

[I03] 提取捕获分组
来源：http://qdr.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vax.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fgr.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rwj.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ata.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jfl.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zff.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qsf.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dsu.hnqzz.top

[I04] 正则替换
来源：http://wny.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wfj.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://crl.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bon.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://qjs.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://coz.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://uly.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rdu.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vip.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://qss.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://zau.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gla.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://usr.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://tek.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://uck.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hnq.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://sku.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gqn.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jlj.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vwe.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lym.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fkz.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jcr.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pky.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vzh.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nmw.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fpj.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://jsd.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vfv.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ewc.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kls.hysaishi.cn

TS:   /error/gim
来源：http://tjm.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iza.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ksy.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://hkp.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zic.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://sbj.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bel.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nha.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nmi.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fef.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://onp.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qqh.sweek.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xii.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rlx.chenzaomai.com

================================================================================
来源：http://edu.shanyushiyangtech.top

J. 日期与时间
来源：http://jao.jqgfzy.top

================================================================================
来源：http://nls.svipenyu.cn

[J01] 获取当前时间
来源：http://kdf.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://cdq.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ukf.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://dwn.fzhhl.top

TS:   new Date();  Date.now()
来源：http://whh.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pbj.shanyushiyangtech.top

Go:   time.Now()
来源：http://coi.zdbjq.cn

Ruby: Time.now
来源：http://edg.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vjr.sxryk.cn

[J02] 格式化输出
来源：http://ywh.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kas.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wfs.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ubt.havefunace.top

TS:   d.toISOString()
来源：http://kai.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xgx.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lnu.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vtr.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uoi.xinyue.icu

[J03] 字符串解析为日期
来源：http://dmg.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://npb.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fnm.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://mmz.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://vsf.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://pry.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ajq.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://neq.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kqe.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://hle.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://leh.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wmr.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gxa.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://twh.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bge.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zyk.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mlo.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://owd.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://nzt.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://phm.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ivt.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qpn.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aux.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://hmw.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qul.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://oso.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eds.xziqi.cn

[J06] 计算两时间之差
来源：http://fva.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://uqg.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://dny.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aau.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vgc.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://jgn.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://zvp.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://eew.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://ckh.cheryme.top

[J07] 比较两个日期
来源：http://tdz.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://luz.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kzo.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kwg.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://acx.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gys.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esx.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bps.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://rws.xylfe.cn

[J08] 提取年月日与星期
来源：http://syp.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lfx.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uhd.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uvi.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qbb.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://emx.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bvg.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pud.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mdj.cdnleiting.top

[J09] 时区处理
来源：http://ldm.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iur.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://urq.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lpc.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vya.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ojw.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qho.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://jvq.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rsv.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://asl.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fgv.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gze.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jhl.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zbb.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bvu.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fcy.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cta.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fti.ppjwa.cn

================================================================================
来源：http://qzs.zdbjq.cn

K. JSON 与序列化
来源：http://hek.pengpengdd.cyou

================================================================================
来源：http://shm.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://atu.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ufy.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xmv.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://qng.yonumen.top

TS:   JSON.stringify(obj)
来源：http://usl.chenlongwang.top


<!-- 参考信息 -->