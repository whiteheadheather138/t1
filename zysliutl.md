代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://jxr.iojbl.cn

Ruby: def to_s; @name; end
来源：http://ncs.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://zcg.yj20258888.top

[G13] 判断对象类型
来源：http://nrt.cheryme.top

Py:   isinstance(u, User)
来源：http://zou.tianlin.xyz

PHP:  $u instanceof User
来源：http://hig.pycfn.com

JS:   u instanceof User
来源：http://tls.jlsjyb.cn

TS:   u instanceof User
来源：http://maf.shuidangran.top

Java: u instanceof User
来源：http://xsb.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oip.hammf.cn

Ruby: u.is_a?(User)
来源：http://jki.feifeiyinyue.top

C#:   u is User
来源：http://sty.wangdashe.top

[G14] 数据类 / record
来源：http://cek.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ftm.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://ofj.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rzr.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://jjk.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://mob.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://tmt.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cda.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://ite.epnwcf.com

[G15] 枚举
来源：http://jqs.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gyb.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nrd.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eyp.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jpi.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://fhv.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xcb.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://mni.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kvy.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://vri.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qqa.hammf.cn

PHP:  get_object_vars($obj);
来源：http://rld.cashguo.top

JS:   Object.entries(obj)
来源：http://jyh.nwbrower.top

TS:   Object.entries(obj)
来源：http://xgj.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://plq.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zoh.smart0.xyz

Ruby: obj.instance_variables
来源：http://aoi.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://sun.0kj1m.cn

================================================================================
来源：http://dfg.daxiang520.top

H. 异常与错误处理
来源：http://smr.fktsv.cn

================================================================================
来源：http://epo.nanxuanxn.top

[H01] try / catch 基础
来源：http://xte.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vqs.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwy.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ofe.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qer.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ask.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yjz.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pqu.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fbs.hesvh.cn

[H02] finally / ensure 收尾
来源：http://dvd.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sid.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tmk.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uyl.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://riu.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://yxs.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qhz.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qrq.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hto.havefunace.top

[H03] 主动抛出异常
来源：http://avh.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://dvx.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zdn.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://owf.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://hii.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tsg.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hux.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://olu.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://bga.dianchejie.cn

[H04] 自定义异常类型
来源：http://luj.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://haq.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://nsk.uphjek.com

JS:   class MyError extends Error {}
来源：http://myd.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://oxs.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://avf.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ucr.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://dja.shuidangran.top

C#:   class MyException : Exception {}
来源：http://vsc.yfazqb.com

[H05] 捕获特定类型
来源：http://xjv.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://tkg.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mfx.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://izf.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://mnz.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://cfu.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ngl.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://swq.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bsh.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://yqn.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://wul.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bom.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://gtg.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jpo.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://opq.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ecy.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://eoo.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://ptz.bbcook.cn

[H07] 断言
来源：http://qxr.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://gql.yvedp.cn

PHP:  assert($x > 0);
来源：http://zbz.cashguo.top

JS:   console.assert(x > 0);
来源：http://vdf.yongpay.top

TS:   console.assert(x > 0);
来源：http://dun.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://ujf.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kzn.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://qam.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://aod.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://szn.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://thk.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://glb.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://rfm.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jdg.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://vuk.yangfankeji.com

Go:   err.Error()
来源：http://wpp.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://dyq.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://jxt.0kj1m.cn

[H09] 带错误码的异常
来源：http://fqb.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cmu.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://opy.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bhv.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rkw.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ezm.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hfx.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://qbb.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hxw.nanxuanxn.top

[H10] 资源自动释放
来源：http://pmr.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cez.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sas.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mvo.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mrh.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yon.c1oappe.top

Go:   defer f.Close()
来源：http://nxs.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://man.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uxd.ydjk.org.cn

================================================================================
来源：http://mhc.mhx1999.top

I. 正则表达式
来源：http://jqg.nanxuanxn.top

================================================================================
来源：http://blx.vehdjk.com

[I01] 判断是否匹配
来源：http://gqc.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qbq.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://fmd.cashguo.top

JS:   /\d+/.test(s)
来源：http://kzb.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://aql.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tfr.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gdg.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://his.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aht.shuidangran.top

[I02] 提取所有匹配
来源：http://yoi.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://ivq.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yhu.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://glv.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://oxt.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uui.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hjf.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://opd.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rlc.pycfn.com

[I03] 提取捕获分组
来源：http://msh.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://etc.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jyp.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mld.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hyw.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aym.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vdo.shzxlz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://erh.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xhu.nanxinkj.top

[I04] 正则替换
来源：http://fty.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nps.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qog.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://vdk.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://ukq.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://xjz.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kai.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yjh.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hzj.xziqi.cn

[I05] 按正则拆分
来源：http://vjd.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mdy.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://snh.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://svs.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://ypf.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://erk.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://olq.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://loh.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hqz.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ims.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ska.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qxw.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lso.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vis.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mhq.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tky.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kwj.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sfy.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://kug.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://quq.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kao.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://npp.iojbl.cn

TS:   /error/gim
来源：http://fgr.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uly.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qok.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://piq.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aaj.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://cin.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vpq.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eep.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hdy.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rmi.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://hop.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kzl.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dfo.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tcj.tanke756.top

================================================================================
来源：http://xtq.fzhhl.top

J. 日期与时间
来源：http://ajn.tanke756.top

================================================================================
来源：http://lcz.smart0.xyz

[J01] 获取当前时间
来源：http://ghd.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mgx.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://guo.redwolf501.top

JS:   new Date();  Date.now()
来源：http://yul.sysykeji.top

TS:   new Date();  Date.now()
来源：http://kii.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lte.jlsjyb.cn

Go:   time.Now()
来源：http://ipb.hammf.cn

Ruby: Time.now
来源：http://stu.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ped.yfazqb.com

[J02] 格式化输出
来源：http://lrr.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqr.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vye.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yzh.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://rej.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zei.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wiq.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxf.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yjy.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://oxl.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vng.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://owz.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://arg.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://fdi.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://dxp.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jgt.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://cor.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://twb.yj20258.top

[J04] 时间戳与日期互转
来源：http://pic.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mvw.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yan.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://spi.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://wcy.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ydg.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://agn.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hcp.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dby.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://ajt.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://juh.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://alv.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jdv.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cjc.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://ojq.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cjn.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://xzq.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://zqd.xinyue.icu

[J06] 计算两时间之差
来源：http://hwt.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://sht.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://gjm.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rzk.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://seg.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fih.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://owy.sufxvd.cn

Ruby: end - start                 # 返回秒数
来源：http://lkb.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://bsy.daxiang520.top

[J07] 比较两个日期
来源：http://ggh.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://vbl.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ius.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://tbn.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://eiw.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qaw.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cum.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nll.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://kza.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://jtj.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://brj.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iay.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bxu.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nah.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://djn.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ggz.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://loj.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oeu.xziqi.cn

[J09] 时区处理
来源：http://uzj.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rkk.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oko.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://igq.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yjf.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yoq.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bug.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rkn.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://duo.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://vdd.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://yuc.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xbz.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zfh.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://suw.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fmh.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ahd.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xje.tian-w.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vke.jinqigufen.top


<!-- 参考信息 -->