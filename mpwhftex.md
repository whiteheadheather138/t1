代发 wailian999

Java: u instanceof User
来源：http://uyd.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://fcg.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://cjd.fktsv.cn

C#:   u is User
来源：http://bbl.uphjek.com

[G14] 数据类 / record
来源：http://fya.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hhz.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://doe.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fvt.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://gbl.fengsongda.top

Java: record User(String name, int age) {}
来源：http://fpk.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://tbt.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lzy.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://osf.shangyingyoupin.top

[G15] 枚举
来源：http://cds.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uyl.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://klt.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rca.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ngo.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://edb.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vjp.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://qgl.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cnm.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://dfl.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://myb.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://rsr.zdbjq.cn

JS:   Object.entries(obj)
来源：http://icm.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://myp.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fgf.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lgh.yuanzhike.top

Ruby: obj.instance_variables
来源：http://xyc.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://ema.jinghuilouyu.cn

================================================================================
来源：http://stq.aibaodan.cn

H. 异常与错误处理
来源：http://grr.jyoumei.cn

================================================================================
来源：http://neh.yfazqb.com

[H01] try / catch 基础
来源：http://jku.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lxk.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mfn.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gjp.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://neu.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eqj.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rvg.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ocs.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ffp.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://gdo.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kzx.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nqj.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rmx.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gax.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://vto.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://rcv.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gkt.hammf.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jkg.gaohongyu789.top

[H03] 主动抛出异常
来源：http://zbz.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://zfb.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pih.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://hjy.hammf.cn

TS:   throw new Error("错误信息");
来源：http://riv.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://avk.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pwo.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rus.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rpy.jiagoushi.top

[H04] 自定义异常类型
来源：http://qos.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://yuo.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://vzj.yuxming.cn

JS:   class MyError extends Error {}
来源：http://yqc.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://alj.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://gxr.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xqt.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://rwf.yj202588.top

C#:   class MyException : Exception {}
来源：http://zvp.nwbrower.top

[H05] 捕获特定类型
来源：http://gta.aibaodan.cn

Py:   except ValueError as e:
来源：http://azx.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wej.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://ukz.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://psi.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://jnp.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rnk.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://qnr.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rgf.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://gfr.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://ifw.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hxw.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://oni.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://lhz.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bue.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vqj.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://soa.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://msc.zhiwuduotai.top

[H07] 断言
来源：http://kjh.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://krt.epnwcf.com

PHP:  assert($x > 0);
来源：http://mly.andypj.xyz

JS:   console.assert(x > 0);
来源：http://ryo.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://mac.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://gcj.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vbh.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://zee.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://lrz.sweek.top

[H08] 获取错误信息与堆栈
来源：http://cij.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://vrq.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vzq.dianchejie.cn

JS:   e.message;  e.stack
来源：http://obh.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ldr.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mhs.fanxiaobao.xyz

Go:   err.Error()
来源：http://utf.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://dph.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://sff.hfpthk.cn

[H09] 带错误码的异常
来源：http://hpp.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ylu.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ksa.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jsv.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wwc.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zyz.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ken.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ndn.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://aji.pengpengdd.cyou

[H10] 资源自动释放
来源：http://htr.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://emg.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ckt.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zdd.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pdg.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://amp.hnxiangtu.top

Go:   defer f.Close()
来源：http://srq.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hvm.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qzf.chenjidiqi.icu

================================================================================
来源：http://lsx.quarkkingdee.top

I. 正则表达式
来源：http://guo.redwolf501.top

================================================================================
来源：http://oax.tarul.cn

[I01] 判断是否匹配
来源：http://scu.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ohd.sjlbkw.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ysr.yvedp.cn

JS:   /\d+/.test(s)
来源：http://hgi.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://pkz.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pkw.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xrv.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://nvb.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jyo.xziqi.cn

[I02] 提取所有匹配
来源：http://qlg.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://rbj.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bia.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wkj.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://xns.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xdb.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://say.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://ydu.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wjz.cashguo.top

[I03] 提取捕获分组
来源：http://fji.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hor.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://saq.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wht.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vds.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://khc.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qws.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zeb.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zyq.daria6918.cn

[I04] 正则替换
来源：http://sfh.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ekn.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dss.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://rjg.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://kvv.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://tum.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gus.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nwi.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://isr.daria6918.cn

[I05] 按正则拆分
来源：http://rbt.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://idm.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kmd.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://wby.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://yoc.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://pvi.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tym.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://rqi.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://msn.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iig.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mlm.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://byn.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://avo.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qmt.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rdj.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xug.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ntu.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gpi.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://zwv.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qao.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rph.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://flc.pengpengdd.cyou

TS:   /error/gim
来源：http://lrb.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ssf.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cdt.pycfn.com

Ruby: s.scan(/error/i)
来源：http://zdk.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://usv.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://krm.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mzb.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://acy.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ufz.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsm.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jze.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rus.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://amx.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ppx.ivvv.top

================================================================================
来源：http://boz.sxryk.cn

J. 日期与时间
来源：http://zfu.tanke756.top

================================================================================
来源：http://hsw.cqqwz.cn

[J01] 获取当前时间
来源：http://plu.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kxj.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cgz.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://cnc.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://wcf.iojbl.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ktc.yonumen.top

Go:   time.Now()
来源：http://qvw.chenjidiqi.icu

Ruby: Time.now
来源：http://plp.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jvb.zdbjq.cn

[J02] 格式化输出
来源：http://yop.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rfo.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xpc.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qnq.pycfn.com

TS:   d.toISOString()
来源：http://hom.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rpu.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rkr.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssv.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ufp.jqgfzy.top

[J03] 字符串解析为日期
来源：http://ifd.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://itn.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qbs.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://qyv.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://xsn.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ife.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tcd.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://uxr.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yze.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://uwf.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wkn.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dru.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://num.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ilu.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zth.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xby.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wlr.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wca.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://qzi.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://cav.chenlongwang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xgy.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://utj.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ayz.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://zyf.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mnh.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://hlr.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://yvt.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://kur.yj20258.top

Py:   (end - start).total_seconds()
来源：http://aqz.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://qxh.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wub.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lyc.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://xoe.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://kep.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://alu.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://awq.zhongyouzk.top

[J07] 比较两个日期
来源：http://bqs.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://zgb.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nky.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zda.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://xew.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xhn.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kiw.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://xfo.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://zfh.zdqjudy.top

[J08] 提取年月日与星期
来源：http://qyn.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xba.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mzi.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hyx.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iky.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jpp.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://utn.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eto.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xsq.xuetiantiany.cn

[J09] 时区处理
来源：http://tds.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kiy.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nas.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://phd.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://atx.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zkg.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lqe.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pfj.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vvv.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://hcw.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://igg.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ski.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://otb.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://buo.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uqj.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aqr.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jmo.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fhd.bbcook.cn

================================================================================
来源：http://gys.yuanzhike.top

K. JSON 与序列化
来源：http://hmh.yfazqb.com

================================================================================
来源：http://bxo.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://uri.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gjt.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jxl.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://fth.yj20258.top

TS:   JSON.stringify(obj)
来源：http://okq.haohaochexian.top


<!-- 参考信息 -->