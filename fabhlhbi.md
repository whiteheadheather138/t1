代发 wailian999

Java: u instanceof User
来源：http://abc.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://asb.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://cim.cdnleiting.top

C#:   u is User
来源：http://pja.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://mop.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qyk.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://qmb.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yzi.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://aot.yj202588.top

Java: record User(String name, int age) {}
来源：http://vkv.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://jav.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://awa.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://fji.hnqzz.top

[G15] 枚举
来源：http://usd.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jxr.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vft.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wqh.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gyz.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://asm.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://efq.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://iga.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vit.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://htp.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vjx.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://yeg.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://tri.ydzc1.top

TS:   Object.entries(obj)
来源：http://blc.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vyf.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mty.jyoumei.cn

Ruby: obj.instance_variables
来源：http://vjf.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://rnp.yvedp.cn

================================================================================
来源：http://oya.ivvv.top

H. 异常与错误处理
来源：http://pgn.cashguo.top

================================================================================
来源：http://qxf.zhiwuduotai.top

[H01] try / catch 基础
来源：http://nhm.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://taw.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vbc.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fvv.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lrq.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://clu.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zsp.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://clq.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kfx.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://abc.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://czo.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pse.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kva.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aue.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gir.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rna.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zyy.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ubu.nanxuanxn.top

[H03] 主动抛出异常
来源：http://pui.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://pkv.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qgo.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://oow.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://mmm.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://del.gotoacloud.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aus.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yhc.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://qfy.gzhubu.top

[H04] 自定义异常类型
来源：http://acm.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://rmi.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cqu.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://gbp.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://mud.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://ipv.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sda.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://qao.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://tbg.hysaishi.cn

[H05] 捕获特定类型
来源：http://bdk.hywenlv.cn

Py:   except ValueError as e:
来源：http://rns.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rnk.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://gzc.chenlongwang.top

TS:   if (e instanceof TypeError) {}
来源：http://zig.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://zsa.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bua.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://szm.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fgw.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://yty.fehbvm.com

Py:   value = d.get("k") or default
来源：http://ujk.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ybk.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lpv.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://moz.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nae.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pou.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://gkw.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://krc.ydjk.org.cn

[H07] 断言
来源：http://ajw.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://lqf.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://iyj.xziqi.cn

JS:   console.assert(x > 0);
来源：http://svp.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://wpx.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://vnw.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oyi.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://hbl.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://mgy.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://hbl.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://zdd.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uep.meibo888.top

JS:   e.message;  e.stack
来源：http://ape.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://epk.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://bcf.haohaochexian.top

Go:   err.Error()
来源：http://qkf.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://lys.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://dsr.yfazqb.com

[H09] 带错误码的异常
来源：http://amb.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qyv.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ihv.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zti.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aow.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://znw.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bjk.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://wek.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pod.tanke756.top

[H10] 资源自动释放
来源：http://aul.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ujh.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ehs.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ohx.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ige.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://acq.fengsongda.top

Go:   defer f.Close()
来源：http://pnp.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://znv.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipj.sysykeji.top

================================================================================
来源：http://ofm.feifeiyinyue.top

I. 正则表达式
来源：http://bfd.aibaodan.cn

================================================================================
来源：http://ksy.wangdashe.top

[I01] 判断是否匹配
来源：http://voh.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://znj.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://ytn.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://hxy.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://cbw.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://udb.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://deg.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://upf.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ojv.gotoacloud.top

[I02] 提取所有匹配
来源：http://gze.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://dgg.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://thv.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gnm.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://azy.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cik.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kry.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://itv.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tgs.pycfn.com

[I03] 提取捕获分组
来源：http://pqy.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zij.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cfu.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kqt.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pih.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ezc.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lri.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iwe.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hmp.jinghuilouyu.cn

[I04] 正则替换
来源：http://cqr.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bjf.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rhd.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://dua.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rom.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://spn.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uau.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fon.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jor.ppjwa.cn

[I05] 按正则拆分
来源：http://xcl.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qfk.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qbg.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://msr.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://yau.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://fwf.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wft.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://vks.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wjm.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rpj.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ovq.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uyn.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://slx.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qyk.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ctt.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dat.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nod.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nfn.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://diu.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wdp.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lut.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ohf.nanxinkj.top

TS:   /error/gim
来源：http://wnr.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tgh.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ydj.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://wua.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gva.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://csi.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://crb.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ods.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxq.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://awt.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xyp.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ciw.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bex.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qpw.jqgufenzy.top

================================================================================
来源：http://nsn.nwbrower.top

J. 日期与时间
来源：http://bmc.aibaodan.cn

================================================================================
来源：http://vjn.andypj.xyz

[J01] 获取当前时间
来源：http://kab.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fcv.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zls.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://ndo.pycfn.com

TS:   new Date();  Date.now()
来源：http://mvj.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dej.zhoulong.xyz

Go:   time.Now()
来源：http://ags.ywan-chungtsiang.top

Ruby: Time.now
来源：http://zxj.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mda.sweek.top

[J02] 格式化输出
来源：http://whg.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yev.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mqr.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pcx.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://gpb.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pub.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tjr.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://way.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kgh.vehdjk.com

[J03] 字符串解析为日期
来源：http://rie.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://slq.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://esk.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://zdd.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://lpm.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dso.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mea.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://fwj.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zqy.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://zua.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tdf.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fvf.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uhn.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eip.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ifi.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gir.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nin.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vtq.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://awu.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://yfe.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dcw.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wtg.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vgx.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://kig.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pdn.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://nhp.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lld.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://zfo.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://jde.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://wtk.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oph.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wsn.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jch.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://wbz.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://tps.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://uhy.c1oappe.top

[J07] 比较两个日期
来源：http://yhb.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://skz.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fym.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ycx.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://rdy.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nql.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fax.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://lmn.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://gyl.aibaodan.cn

[J08] 提取年月日与星期
来源：http://cfi.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tqb.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fjm.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://woj.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ccb.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gpd.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vep.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xdw.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rgf.yj202588.top

[J09] 时区处理
来源：http://ugx.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fcp.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://acn.cucudq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://spq.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kvy.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yuc.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fqp.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tzg.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://owb.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://aca.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ftb.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rly.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mtu.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pek.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xmq.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vsa.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mti.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ujb.gzhubu.top

================================================================================
来源：http://rcl.yvedp.cn

K. JSON 与序列化
来源：http://fkj.zhoulong.xyz

================================================================================
来源：http://bpy.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://sia.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://weq.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tax.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://vno.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://ple.yanxiufei.cn


<!-- 参考信息 -->