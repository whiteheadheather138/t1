代发 wailian999

Java: interface Shape { double area(); }
来源：http://hxz.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://fdd.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cpf.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://azf.jinghuilouyu.cn

[G10] 访问控制
来源：http://vcp.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://yda.xinyue.icu

PHP:  public / protected / private
来源：http://ndw.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://kvg.zdbjq.cn

TS:   public / protected / private
来源：http://xua.ivvv.top

Java: public / protected / private / 默认包级
来源：http://gic.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ojh.bbcook.cn

Ruby: public / protected / private
来源：http://teg.hnqzz.top

C#:   public / protected / private / internal
来源：http://lsb.daria6918.cn

[G11] getter / setter
来源：http://woq.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://vdl.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rjk.hnqzz.top

JS:   get name() { return this._name; }
来源：http://kdd.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://psj.xziqi.cn

Java: public String getName() { return name; }
来源：http://eyn.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvr.guannengcc.top

Ruby: attr_accessor :name
来源：http://mcb.daxiang520.top

C#:   public string Name { get; set; }
来源：http://cug.sweek.top

[G12] 对象转字符串
来源：http://fue.tarul.cn

Py:   def __str__(self): return self.name
来源：http://kbj.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kll.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://gow.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://vgn.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://fdv.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://dbx.daria6918.cn

Ruby: def to_s; @name; end
来源：http://ssn.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://pkb.epnwcf.com

[G13] 判断对象类型
来源：http://eag.hcnkem.com

Py:   isinstance(u, User)
来源：http://yvp.jlsjyb.cn

PHP:  $u instanceof User
来源：http://pct.bbcook.cn

JS:   u instanceof User
来源：http://jbg.jianghu66.top

TS:   u instanceof User
来源：http://cpu.jlsjyb.cn

Java: u instanceof User
来源：http://zvr.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xoe.havefunace.top

Ruby: u.is_a?(User)
来源：http://zza.meibo888.top

C#:   u is User
来源：http://hzy.cashguo.top

[G14] 数据类 / record
来源：http://bhv.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uxj.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://fon.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://hpf.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://jen.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://ekf.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://sgs.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rxg.havefunace.top

C#:   record User(string Name, int Age);
来源：http://wko.hfpthk.cn

[G15] 枚举
来源：http://qwz.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ror.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gmb.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vjy.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jhy.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://slw.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uvn.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://cil.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mow.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://hzs.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zdk.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://rgm.jiagoushi.top

JS:   Object.entries(obj)
来源：http://ckm.c1oappe.top

TS:   Object.entries(obj)
来源：http://bih.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pvb.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vzf.tanke756.top

Ruby: obj.instance_variables
来源：http://mzw.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dfr.jqgufenzy.top

================================================================================
来源：http://unw.tarul.cn

H. 异常与错误处理
来源：http://wgi.xylfe.cn

================================================================================
来源：http://wlb.zhongyouzk.top

[H01] try / catch 基础
来源：http://kyy.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nom.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pzn.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://irz.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xso.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ksy.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hrh.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://plr.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wza.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://mjs.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ike.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dam.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zhg.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vvo.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://uur.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://teh.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://uro.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lwj.zhoulong.xyz

[H03] 主动抛出异常
来源：http://otb.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://crq.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mju.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://vcj.tanke756.top

TS:   throw new Error("错误信息");
来源：http://pvo.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rjf.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jmw.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xyx.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://csz.jianghu66.top

[H04] 自定义异常类型
来源：http://gay.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://fnh.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xmh.hnqzz.top

JS:   class MyError extends Error {}
来源：http://kob.andypj.xyz

TS:   class MyError extends Error {}
来源：http://bnv.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://tuq.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rre.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://qro.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://rto.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://buh.hesvh.cn

Py:   except ValueError as e:
来源：http://jar.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oja.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://gij.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://grc.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://szr.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vus.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://dxq.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gtp.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://xpg.yfazqb.com

Py:   value = d.get("k") or default
来源：http://vzr.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://dma.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://ufb.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gsh.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jsb.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qrn.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://zun.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://tao.yanxiufei.cn

[H07] 断言
来源：http://afn.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://gej.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://yyj.redwolf501.top

JS:   console.assert(x > 0);
来源：http://tdz.andypj.xyz

TS:   console.assert(x > 0);
来源：http://xqa.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://ezi.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nyv.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://coq.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://hxn.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://wsu.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://goc.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uev.yangfankeji.com

JS:   e.message;  e.stack
来源：http://csk.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gui.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tbp.kuanghao11.cn

Go:   err.Error()
来源：http://ibn.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://pyo.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://vrc.hnqzz.top

[H09] 带错误码的异常
来源：http://vxb.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ege.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qix.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sgc.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jpd.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://opm.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ckt.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://fej.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mlt.zhongyouzk.top

[H10] 资源自动释放
来源：http://mrv.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://izg.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://brc.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tmo.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qzz.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gqp.sxryk.cn

Go:   defer f.Close()
来源：http://vqw.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xew.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nux.meibo888.top

================================================================================
来源：http://stn.jqgfzy.top

I. 正则表达式
来源：http://xhk.nwbrower.top

================================================================================
来源：http://cqg.guannengcc.top

[I01] 判断是否匹配
来源：http://oln.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ivk.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://hmi.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://djn.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://rsa.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hgf.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tsa.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://gkl.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dps.dianchejie.cn

[I02] 提取所有匹配
来源：http://jdz.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://zyl.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xqq.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rom.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://yud.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tpi.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zrl.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://xyc.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fek.fengsongda.top

[I03] 提取捕获分组
来源：http://neu.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sly.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nmi.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://prd.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kzo.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yxq.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kph.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lix.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dak.ybcxt.top

[I04] 正则替换
来源：http://ytn.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sud.hesvh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yan.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://imb.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://jiw.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://hnb.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vbf.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dor.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sub.fehbvm.com

[I05] 按正则拆分
来源：http://jbs.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wdw.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dsd.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://zkt.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://gtw.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://lde.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oem.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://lfz.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://chq.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aoc.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gpo.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mus.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://puz.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdz.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pfj.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bsk.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pkr.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kap.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://qpw.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ojq.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mqw.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rxc.aizwys.cn

TS:   /error/gim
来源：http://gnn.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://glj.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mph.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://xxh.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qec.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://mvk.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://php.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ibu.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vie.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mrk.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://upe.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jux.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ruz.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kas.pycfn.com

================================================================================
来源：http://ssf.hnxiangtu.top

J. 日期与时间
来源：http://leo.xuetiantiany.cn

================================================================================
来源：http://xlu.hfpthk.cn

[J01] 获取当前时间
来源：http://ihk.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kch.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hzb.daria6918.cn

JS:   new Date();  Date.now()
来源：http://zon.yueranfly.top

TS:   new Date();  Date.now()
来源：http://jra.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nrk.cashguo.top

Go:   time.Now()
来源：http://gss.ppjwa.cn

Ruby: Time.now
来源：http://sfk.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://obw.jinqigufen.top

[J02] 格式化输出
来源：http://gll.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sky.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bfm.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://avx.yj20258888.top

TS:   d.toISOString()
来源：http://krx.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bny.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nbr.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ihj.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nlj.yonumen.top

[J03] 字符串解析为日期
来源：http://hto.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://feb.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vvd.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://vvf.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://lke.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://pym.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dld.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://hgd.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kof.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://wkl.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cij.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qme.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zvv.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pvc.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://roa.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jww.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pxs.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lij.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://pyo.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://qgu.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dvj.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nif.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dcr.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://cld.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wwb.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://rmg.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://izx.xinyue.icu

[J06] 计算两时间之差
来源：http://gji.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://ulc.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://duc.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yfq.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xbu.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jnf.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://mvn.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://exp.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://fud.sweek.top

[J07] 比较两个日期
来源：http://usu.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://wrt.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://efm.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://ijv.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://dws.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://apx.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bqe.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://tdc.jlsjyb.cn


<!-- 参考信息 -->