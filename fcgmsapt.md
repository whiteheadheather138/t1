代发 wailian999

C#:   public / protected / private / internal
来源：http://isv.52xcode.cn

[G11] getter / setter
来源：http://tpu.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://rbl.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ibe.fktsv.cn

JS:   get name() { return this._name; }
来源：http://gjd.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://sye.iojbl.cn

Java: public String getName() { return name; }
来源：http://aeh.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://agp.bjfxy.top

Ruby: attr_accessor :name
来源：http://lpq.zycfv.cn

C#:   public string Name { get; set; }
来源：http://ijg.cheryme.top

[G12] 对象转字符串
来源：http://nde.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://xur.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pkp.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://web.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://dcb.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://xdm.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://thh.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://qzr.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://ifv.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://twm.sufxvd.cn

Py:   isinstance(u, User)
来源：http://vos.jianghu66.top

PHP:  $u instanceof User
来源：http://moj.9152youxi.cn

JS:   u instanceof User
来源：http://syt.chenjidiqi.icu

TS:   u instanceof User
来源：http://naj.tianlin.xyz

Java: u instanceof User
来源：http://dxq.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mix.zhiwuduotai.top

Ruby: u.is_a?(User)
来源：http://lha.meibo888.top

C#:   u is User
来源：http://jzy.sjlbkw.cn

[G14] 数据类 / record
来源：http://lqk.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rde.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://lph.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oxr.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://dxs.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://psx.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://wyl.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qlg.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://obt.yfazqb.com

[G15] 枚举
来源：http://xor.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xbl.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zhy.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lit.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kfj.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://fxg.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hze.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://qiq.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djv.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://nzu.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cct.316326.xyz

PHP:  get_object_vars($obj);
来源：http://xrs.ydzc1.top

JS:   Object.entries(obj)
来源：http://giy.xylfe.cn

TS:   Object.entries(obj)
来源：http://qza.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ywt.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cpl.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://gxf.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://xgi.chenlongwang.top

================================================================================
来源：http://kqe.sjlbkw.cn

H. 异常与错误处理
来源：http://bae.haohaochexian.top

================================================================================
来源：http://znu.andypj.xyz

[H01] try / catch 基础
来源：http://llo.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://psi.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ehp.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xdx.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgp.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://afe.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aox.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rce.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rds.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://zfx.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jxb.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://guf.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xhi.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dqa.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://yih.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uwv.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hij.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rmk.daria6918.cn

[H03] 主动抛出异常
来源：http://igj.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://vem.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lbc.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://apx.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://wwz.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vqz.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vbs.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://suz.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://ovj.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://juh.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://ldj.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qhl.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://iho.xylfe.cn

TS:   class MyError extends Error {}
来源：http://xht.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://vlj.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dcz.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://kjs.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://ioa.cashguo.top

[H05] 捕获特定类型
来源：http://xtd.yangfankeji.com

Py:   except ValueError as e:
来源：http://akw.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zez.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://xtk.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://xkn.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://vrk.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gfw.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://gza.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aim.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://lew.fzhhl.top

Py:   value = d.get("k") or default
来源：http://dtd.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sbq.jyoumei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bnu.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gzg.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gmd.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://llx.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://zmj.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://vqv.jinqigfzy.top

[H07] 断言
来源：http://rea.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://ygi.aibaodan.cn

PHP:  assert($x > 0);
来源：http://bxp.316326.xyz

JS:   console.assert(x > 0);
来源：http://xyt.tanke756.top

TS:   console.assert(x > 0);
来源：http://bne.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://gnf.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wsa.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ogl.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://avo.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://mtv.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://jnb.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jnf.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://vve.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kcm.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://wxp.9152youxi.cn

Go:   err.Error()
来源：http://dum.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://smv.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://qoo.gogol.net.cn

[H09] 带错误码的异常
来源：http://krz.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://txc.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rvf.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pjq.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lxv.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ewq.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ruq.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://ftw.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ynz.svipenyu.cn

[H10] 资源自动释放
来源：http://fpe.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://exb.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rix.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ixa.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ltm.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://awt.yj202588.top

Go:   defer f.Close()
来源：http://jcj.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ytj.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jfv.nanxinkj.top

================================================================================
来源：http://krr.hnxiangtu.top

I. 正则表达式
来源：http://wxf.jianghu66.top

================================================================================
来源：http://qxw.9152youxi.cn

[I01] 判断是否匹配
来源：http://ous.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fci.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wco.ydzc1.top

JS:   /\d+/.test(s)
来源：http://orc.sweek.top

TS:   /\d+/.test(s)
来源：http://mak.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lvh.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://czh.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://kvf.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wtv.nanxuanxn.top

[I02] 提取所有匹配
来源：http://bun.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://ncj.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ahi.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hyz.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://hgu.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://osu.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hfa.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://vte.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://clp.mhx1999.top

[I03] 提取捕获分组
来源：http://sxz.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pck.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ytr.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tyl.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ygr.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ljf.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://erm.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oha.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://scb.zhoulong.xyz

[I04] 正则替换
来源：http://cci.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ipi.havefunace.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tsk.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://vhf.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ffc.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ppj.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://oca.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://irc.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cbl.tianlin.xyz

[I05] 按正则拆分
来源：http://god.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qlu.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uzo.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://ajq.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://aqo.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://zlg.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kco.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hvj.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uaq.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hhh.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://emz.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uea.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kje.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://idj.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://opf.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wnw.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vuc.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dus.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://jyp.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iwe.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kye.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ezk.yj202588.top

TS:   /error/gim
来源：http://lcf.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://idz.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bzq.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://lmx.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zju.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://mnw.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rzq.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xfi.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mdl.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ilk.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://rcd.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cxz.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fqd.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wvy.fanxiaobao.xyz

================================================================================
来源：http://grj.xingfuxueyuan.xyz

J. 日期与时间
来源：http://fwb.jiagoushi.top

================================================================================
来源：http://mku.hcnkem.com

[J01] 获取当前时间
来源：http://kmg.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bdi.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://upp.cheryme.top

JS:   new Date();  Date.now()
来源：http://tqr.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://rsi.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://avo.feifeiyinyue.top

Go:   time.Now()
来源：http://vvj.gogol.net.cn

Ruby: Time.now
来源：http://qpt.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ntb.hammf.cn

[J02] 格式化输出
来源：http://xag.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovq.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cqi.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ffk.gzhubu.top

TS:   d.toISOString()
来源：http://ygd.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oja.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kcq.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rsd.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mnd.cashguo.top

[J03] 字符串解析为日期
来源：http://zyk.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://epz.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zyr.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://gkk.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://yim.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://nbm.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nxc.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://cgh.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kju.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://kyu.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://msj.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cmb.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tpl.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mds.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://grj.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vzj.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wyv.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iem.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://zjd.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://ljf.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qta.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhl.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhx.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://osv.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fjt.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://rcz.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://hkr.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://mto.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://edo.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://lkr.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nbg.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dmu.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://giu.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://tpj.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://sii.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://pof.meibo888.top

[J07] 比较两个日期
来源：http://lzv.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://dkp.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofi.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://nxm.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://wen.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dta.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://avw.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://rtm.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://nco.jinqigufen.top

[J08] 提取年月日与星期
来源：http://qjd.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://niv.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kjs.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://txa.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dht.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ppk.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://caj.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mfs.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vkx.shanyushiyangtech.top

[J09] 时区处理
来源：http://xwu.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pcv.zdqjudy.top


<!-- 参考信息 -->