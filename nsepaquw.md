代发 wailian999

Py:   isinstance(u, User)
来源：http://vot.tianlin.xyz

PHP:  $u instanceof User
来源：http://yte.hnxiangtu.top

JS:   u instanceof User
来源：http://lhq.hywenlv.cn

TS:   u instanceof User
来源：http://yyu.yj20258.top

Java: u instanceof User
来源：http://ffk.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zoz.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://imd.fzhhl.top

C#:   u is User
来源：http://sgw.fengsongda.top

[G14] 数据类 / record
来源：http://lse.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://keg.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://cxi.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://vmh.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://xoh.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://hba.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://qmb.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sme.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://ubu.nwbrower.top

[G15] 枚举
来源：http://wry.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dyi.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pla.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zbr.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pak.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://igu.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cej.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://pba.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://twi.tarul.cn

[G16] 对象转数组 / 字典
来源：http://bjo.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fbw.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://nth.yuanzhike.top

JS:   Object.entries(obj)
来源：http://zlc.hesvh.cn

TS:   Object.entries(obj)
来源：http://vib.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wne.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tnb.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://taa.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://pzg.meibo888.top

================================================================================
来源：http://foe.sufxvd.cn

H. 异常与错误处理
来源：http://pba.yj202588.top

================================================================================
来源：http://pmu.hcnkem.com

[H01] try / catch 基础
来源：http://reb.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bpq.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rnr.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mob.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hva.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xkc.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mxi.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xtv.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uyf.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://izl.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://ebr.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vxz.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yto.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ise.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://vge.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ncv.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://atp.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tdh.yfazqb.com

[H03] 主动抛出异常
来源：http://isw.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://bqc.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cyt.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://rqy.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://jxg.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://cod.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://prs.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tqp.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://lmi.aibaodan.cn

[H04] 自定义异常类型
来源：http://xol.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://zlm.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://qhr.yj20258888.top

JS:   class MyError extends Error {}
来源：http://ywf.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://mcz.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://mab.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yau.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://fxr.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://qwg.zhongyouzk.top

[H05] 捕获特定类型
来源：http://nab.andypj.xyz

Py:   except ValueError as e:
来源：http://cki.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aed.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://ijh.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://spt.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://fky.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ire.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://dgg.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bjv.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://aen.jianghu66.top

Py:   value = d.get("k") or default
来源：http://ots.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pxy.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dxc.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://bqg.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kpf.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://thp.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://hka.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://ymf.zhoulong.xyz

[H07] 断言
来源：http://nmi.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://zwb.birdmap.top

PHP:  assert($x > 0);
来源：http://sbu.hnqzz.top

JS:   console.assert(x > 0);
来源：http://myt.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://gsg.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://rur.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ujd.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ayx.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://yif.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://ijn.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://ykg.sjlbkw.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xtd.hysaishi.cn

JS:   e.message;  e.stack
来源：http://auz.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xdy.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ufr.fehbvm.com

Go:   err.Error()
来源：http://qoy.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://qyz.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://dtl.pycfn.com

[H09] 带错误码的异常
来源：http://oan.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gmj.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://npw.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dri.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dee.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://raq.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iwh.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fep.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ztz.nanxinkj.top

[H10] 资源自动释放
来源：http://wod.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mzm.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wei.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sku.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sqh.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ykd.pengpengdd.cyou

Go:   defer f.Close()
来源：http://pjx.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lhe.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yiz.cqqwz.cn

================================================================================
来源：http://tys.hcnkem.com

I. 正则表达式
来源：http://rym.ivvv.top

================================================================================
来源：http://icc.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://iaz.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vgu.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ngr.ybcxt.top

JS:   /\d+/.test(s)
来源：http://udz.c1oappe.top

TS:   /\d+/.test(s)
来源：http://tui.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gkm.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gkw.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://vzq.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nez.xziqi.cn

[I02] 提取所有匹配
来源：http://wrm.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://uhn.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ozu.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zkz.pycfn.com

TS:   s.match(/\d+/g)
来源：http://btp.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mwi.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eca.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://pli.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rey.fengsongda.top

[I03] 提取捕获分组
来源：http://wys.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kzi.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://par.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eyc.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rok.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oit.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wgf.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iez.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ati.gzhubu.top

[I04] 正则替换
来源：http://ayb.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bml.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iyc.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://dyu.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cxm.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cak.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nlp.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hni.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vdd.fktsv.cn

[I05] 按正则拆分
来源：http://gwr.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ggu.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://typ.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://twl.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://pxy.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://iej.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aig.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://dwj.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://niv.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://miy.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zpe.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uxu.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhr.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://exp.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ima.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vkk.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kje.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hzy.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://tuw.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jtb.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://amc.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cfj.jlsjyb.cn

TS:   /error/gim
来源：http://pev.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sfz.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fta.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://pjm.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://saz.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://owj.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lvp.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://szy.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qrx.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yuj.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rar.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gsv.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hzq.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qgh.yvedp.cn

================================================================================
来源：http://zor.ywan-chungtsiang.top

J. 日期与时间
来源：http://fhh.tianlin.xyz

================================================================================
来源：http://ydu.guowangkeji.top

[J01] 获取当前时间
来源：http://msd.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ihe.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eau.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://nto.tanke756.top

TS:   new Date();  Date.now()
来源：http://vgl.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ggf.uphjek.com

Go:   time.Now()
来源：http://tgh.9152youxi.cn

Ruby: Time.now
来源：http://yox.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fjv.shangyingyoupin.top

[J02] 格式化输出
来源：http://rbm.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yay.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jee.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vpp.bbcook.cn

TS:   d.toISOString()
来源：http://vvx.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://now.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nyk.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rso.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xgb.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://ftx.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tta.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://svb.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://bwm.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://wkb.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wyq.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vpx.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://gfw.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qds.vehdjk.com

[J04] 时间戳与日期互转
来源：http://mjs.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zqe.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yrw.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trk.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mbl.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kak.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvy.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgo.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://shj.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://vae.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://vxu.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pnq.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfq.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jwq.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://jjh.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ovt.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://fbd.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://ovf.zhijiandao.cn

[J06] 计算两时间之差
来源：http://aww.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://giw.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://byp.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nin.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bmj.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://tbs.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://lto.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://fmy.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://zhp.chenjidiqi.icu

[J07] 比较两个日期
来源：http://kpi.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://smy.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xdi.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ack.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ncc.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ruz.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uwm.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://iir.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://ttu.aizwys.cn

[J08] 提取年月日与星期
来源：http://syo.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hgv.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://knv.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://idg.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lss.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yqz.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hfr.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bjy.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tac.cqqwz.cn

[J09] 时区处理
来源：http://lhv.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vad.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://elq.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qdw.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asl.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xqj.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dwl.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ris.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uzi.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://aam.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://exp.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://opf.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lbv.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://etk.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ubc.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pnq.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://imk.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pzb.nanxuanxn.top

================================================================================
来源：http://bsn.yuanzhike.top

K. JSON 与序列化
来源：http://nns.hammf.cn

================================================================================
来源：http://ihn.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://lxt.haohaochexian.top


<!-- 参考信息 -->