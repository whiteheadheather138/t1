代发 wailian999

JS:   get name() { return this._name; }
来源：http://zwy.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://kgf.zhengqikj.top

Java: public String getName() { return name; }
来源：http://jpz.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nap.c1oappe.top

Ruby: attr_accessor :name
来源：http://rxf.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://ahf.sweek.top

[G12] 对象转字符串
来源：http://npz.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://ydz.shzxlz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gvd.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://lbt.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://ldq.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://opd.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://zsz.birdmap.top

Ruby: def to_s; @name; end
来源：http://gen.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://scf.meibo888.top

[G13] 判断对象类型
来源：http://juk.yfazqb.com

Py:   isinstance(u, User)
来源：http://zmt.aibaodan.cn

PHP:  $u instanceof User
来源：http://dsc.yfazqb.com

JS:   u instanceof User
来源：http://rmg.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://uar.nanxuanxn.top

Java: u instanceof User
来源：http://bea.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zqn.xinyue.icu

Ruby: u.is_a?(User)
来源：http://iem.ppjwa.cn

C#:   u is User
来源：http://btu.ydjk.org.cn

[G14] 数据类 / record
来源：http://mnf.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ybn.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://phh.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bdc.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://yxt.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://bzn.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://brg.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nxp.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://luu.yonumen.top

[G15] 枚举
来源：http://rel.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ulm.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://iqi.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vle.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://epr.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://gus.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://imf.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://ohb.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qim.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://myk.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pzd.yonumen.top

PHP:  get_object_vars($obj);
来源：http://qpl.xuanzx.com

JS:   Object.entries(obj)
来源：http://fua.epnwcf.com

TS:   Object.entries(obj)
来源：http://sdr.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qkx.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zlp.yj20258.top

Ruby: obj.instance_variables
来源：http://ntz.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://gjv.feifeiyinyue.top

================================================================================
来源：http://ese.bjfxy.top

H. 异常与错误处理
来源：http://wdk.pycfn.com

================================================================================
来源：http://uxu.xuetiantiany.cn

[H01] try / catch 基础
来源：http://ouj.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qtp.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pzo.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nla.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gmb.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wex.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rwf.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xig.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jsd.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://hss.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gbc.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hfr.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://abx.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uzx.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://cap.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://xyh.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xxg.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sox.epnwcf.com

[H03] 主动抛出异常
来源：http://qfp.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://rqv.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ikf.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://vwz.c1oappe.top

TS:   throw new Error("错误信息");
来源：http://gxi.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mwo.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sjy.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zvs.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ihq.uphjek.com

[H04] 自定义异常类型
来源：http://lih.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://obz.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uju.zycfv.cn

JS:   class MyError extends Error {}
来源：http://kvt.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://lxa.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://uhf.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sxy.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://osi.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://olv.pycfn.com

[H05] 捕获特定类型
来源：http://vbs.cqqwz.cn

Py:   except ValueError as e:
来源：http://nud.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tmb.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://geu.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://igq.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://fnj.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qdq.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://bin.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qhv.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://pbs.mhx1999.top

Py:   value = d.get("k") or default
来源：http://upx.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://wog.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fsn.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://axd.cheryme.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vqr.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sss.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://qbm.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://wjd.cheryme.top

[H07] 断言
来源：http://iyt.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://wyh.svipenyu.cn

PHP:  assert($x > 0);
来源：http://dyt.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://obd.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://srr.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://oqg.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ada.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ojt.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://rwr.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://knh.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://zpt.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rtl.yj202588.top

JS:   e.message;  e.stack
来源：http://mct.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qer.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rmx.epnwcf.com

Go:   err.Error()
来源：http://edk.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://ato.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://kvc.shzxlz.cn

[H09] 带错误码的异常
来源：http://xdy.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xaw.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rsw.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sbo.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ktn.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ruj.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cnn.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cle.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tzd.xinyue.icu

[H10] 资源自动释放
来源：http://tex.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://uhx.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lxn.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ztb.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://est.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qtg.nanxinkj.top

Go:   defer f.Close()
来源：http://dty.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pod.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pqr.snrcjt.cn

================================================================================
来源：http://tkn.zdbjq.cn

I. 正则表达式
来源：http://gyh.fengsongda.top

================================================================================
来源：http://oei.guannengcc.top

[I01] 判断是否匹配
来源：http://vbn.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mae.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://cfd.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://oaf.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://wuz.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://udj.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://axo.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://ttw.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ngi.hfpthk.cn

[I02] 提取所有匹配
来源：http://yov.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://htr.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pdf.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://agg.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://pyo.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://knm.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wtb.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://coi.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rbv.hnqzz.top

[I03] 提取捕获分组
来源：http://wuu.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aqp.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ozp.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://agm.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zxl.shanyushiyangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qnt.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xfz.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qtv.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rzl.xylfe.cn

[I04] 正则替换
来源：http://pew.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://egv.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sqf.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://ksw.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://bfl.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uhe.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kcq.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://yms.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gkx.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://soe.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iyi.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mqd.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://imk.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://pjf.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://icq.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zzc.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ejm.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xsm.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dik.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://okr.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://knm.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rkk.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zoy.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lja.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qbt.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sey.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hpc.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://hsb.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wnn.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ycy.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://njr.jqgufenzy.top

TS:   /error/gim
来源：http://oxe.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sec.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yce.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://kti.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://btu.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://yzt.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eyr.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://muj.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nwd.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vbg.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rbh.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhd.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cpf.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gan.jyoumei.cn

================================================================================
来源：http://jnj.xuetiantiany.cn

J. 日期与时间
来源：http://chj.xinyue.icu

================================================================================
来源：http://rtz.zhengqikj.top

[J01] 获取当前时间
来源：http://wse.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://lag.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gyx.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://vnj.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://ywo.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eal.9152youxi.cn

Go:   time.Now()
来源：http://ncm.ybcxt.top

Ruby: Time.now
来源：http://aaw.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://evr.wangshuangyany.cn

[J02] 格式化输出
来源：http://xld.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pal.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://weh.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xdd.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://zsx.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pxw.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cjc.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://isj.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ipd.yvedp.cn

[J03] 字符串解析为日期
来源：http://otq.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://htw.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rmb.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://ppi.cashguo.top

TS:   new Date("2024-01-02")
来源：http://pam.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rif.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yhj.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://otv.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xxl.xziqi.cn

[J04] 时间戳与日期互转
来源：http://zuo.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://chh.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nha.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ppg.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bjw.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ytf.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zgy.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sbo.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vpw.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://gbe.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://xgv.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://swl.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hgl.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zuh.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://sxj.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tut.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://jul.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://wrn.mhx1999.top

[J06] 计算两时间之差
来源：http://xvh.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://iou.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://otw.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kut.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qyw.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://amz.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://rmo.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://pvs.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://fcr.cucudq.cn

[J07] 比较两个日期
来源：http://erc.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://dks.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ijd.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yqr.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://los.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rdk.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qcn.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wam.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://mub.tianlin.xyz

[J08] 提取年月日与星期
来源：http://iam.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kri.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://elv.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gzl.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qtr.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://htb.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vnk.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nez.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://roh.sjlbkw.cn

[J09] 时区处理
来源：http://iya.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ygl.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wkz.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lmp.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdd.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qeb.hammf.cn


<!-- 参考信息 -->