代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://qip.gotoacloud.top

Ruby: def self.f; end
来源：http://iaa.yvedp.cn

C#:   public static void F() {}
来源：http://xod.yueranfly.top

[G09] 接口 / 抽象类
来源：http://czo.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://boo.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://nnx.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://afw.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://zro.sxryk.cn

Java: interface Shape { double area(); }
来源：http://kyn.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://jvo.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hza.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://aob.epnwcf.com

[G10] 访问控制
来源：http://all.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://dbl.ehwqpu.com

PHP:  public / protected / private
来源：http://cql.fengsongda.top

JS:   #private 字段；其余公开
来源：http://keh.bjfxy.top

TS:   public / protected / private
来源：http://ttc.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://bwu.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zfo.pycfn.com

Ruby: public / protected / private
来源：http://hyc.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://tfj.andypj.xyz

[G11] getter / setter
来源：http://rrt.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://lqk.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xza.vehdjk.com

JS:   get name() { return this._name; }
来源：http://bqi.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://tbc.bbcook.cn

Java: public String getName() { return name; }
来源：http://fgi.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nuf.fengsongda.top

Ruby: attr_accessor :name
来源：http://ozs.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://eyt.pengpengdd.cyou

[G12] 对象转字符串
来源：http://fig.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://hkc.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://khr.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://zxm.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://ftn.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://jwh.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://qqk.andypj.xyz

Ruby: def to_s; @name; end
来源：http://kyb.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://xaz.pengpengdd.cyou

[G13] 判断对象类型
来源：http://euk.hysaishi.cn

Py:   isinstance(u, User)
来源：http://tja.hnxiangtu.top

PHP:  $u instanceof User
来源：http://wco.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://kcp.fehbvm.com

TS:   u instanceof User
来源：http://hgl.jlsjyb.cn

Java: u instanceof User
来源：http://kjz.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://bcy.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://wqh.jlsjyb.cn

C#:   u is User
来源：http://hfp.shangyingyoupin.top

[G14] 数据类 / record
来源：http://fng.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ben.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://rde.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jjd.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://zbt.52xcode.cn

Java: record User(String name, int age) {}
来源：http://wxa.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://tvg.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dbm.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://ddh.shuidangran.top

[G15] 枚举
来源：http://ofy.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://urr.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vrw.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bvl.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ylg.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://opk.chenlongwang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kqw.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://alv.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xgd.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://eut.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wqp.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://dyl.tianlin.xyz

JS:   Object.entries(obj)
来源：http://pqp.zycfv.cn

TS:   Object.entries(obj)
来源：http://xcs.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://avx.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cpl.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://hqa.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://vcd.shanyushiyangtech.top

================================================================================
来源：http://bpw.snrcjt.cn

H. 异常与错误处理
来源：http://wmc.daxiang520.top

================================================================================
来源：http://mzk.gogol.net.cn

[H01] try / catch 基础
来源：http://zpb.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hxi.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gja.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ypa.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yez.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://igd.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qsn.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jyf.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qrv.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://lsi.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://zzj.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cnc.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rxj.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dwp.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tsh.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://rtu.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://giw.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pfc.yvedp.cn

[H03] 主动抛出异常
来源：http://scb.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://xyu.vqdsnc.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nhi.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://vfx.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://rso.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://jmf.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oyn.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xkm.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://qgg.chenzaomai.com

[H04] 自定义异常类型
来源：http://ilx.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://xdp.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vjp.vehdjk.com

JS:   class MyError extends Error {}
来源：http://arb.cheryme.top

TS:   class MyError extends Error {}
来源：http://ekm.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://fmb.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://egj.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://afo.c1oappe.top

C#:   class MyException : Exception {}
来源：http://oir.kuanghao11.cn

[H05] 捕获特定类型
来源：http://not.yuanzhike.top

Py:   except ValueError as e:
来源：http://akz.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://koa.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://nml.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://wqg.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://uif.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://whz.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://fco.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cud.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://flf.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://dgd.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://div.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://ing.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uep.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mqw.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sfu.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://gvo.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://lad.nanxuanxn.top

[H07] 断言
来源：http://miu.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://ves.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://dga.epnwcf.com

JS:   console.assert(x > 0);
来源：http://yzd.vehdjk.com

TS:   console.assert(x > 0);
来源：http://srt.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://qpc.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rdl.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://age.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://oth.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://agy.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://urp.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ipg.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://whx.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://vgg.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://snz.yanxiufei.cn

Go:   err.Error()
来源：http://gwz.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://cdo.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://gne.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://lnf.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gcc.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://opn.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yug.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vcr.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vhz.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xmw.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://ptu.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ijz.feifeiyinyue.top

[H10] 资源自动释放
来源：http://mcy.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://iue.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ivc.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kou.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ghu.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://obm.yonumen.top

Go:   defer f.Close()
来源：http://yrx.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nvv.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mqv.nanxuanxn.top

================================================================================
来源：http://xey.ppjwa.cn

I. 正则表达式
来源：http://nxd.cucudq.cn

================================================================================
来源：http://cvg.ppjwa.cn

[I01] 判断是否匹配
来源：http://jyc.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lxb.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://ssk.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://hhc.tarul.cn

TS:   /\d+/.test(s)
来源：http://ylz.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zym.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zrz.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://pph.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://akl.yj202588.top

[I02] 提取所有匹配
来源：http://rcx.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://sja.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cea.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vom.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://nar.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dqv.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ccr.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://wks.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qbd.tarul.cn

[I03] 提取捕获分组
来源：http://xxa.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cpl.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://erk.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hcc.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fuh.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wia.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sub.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lfr.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oju.ydzc1.top

[I04] 正则替换
来源：http://adk.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ukz.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpp.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://boq.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://mam.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://tyi.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://qir.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yky.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jec.ydjk.org.cn

[I05] 按正则拆分
来源：http://ike.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vsd.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sec.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://btf.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://pcq.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://rwm.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ejk.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://nuw.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nco.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hed.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wtk.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eoi.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sxd.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zqb.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jlm.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oxj.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ngt.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tzt.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://zrh.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xkj.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://six.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zjq.jqgufenzy.top

TS:   /error/gim
来源：http://isx.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wwk.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mci.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://glz.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://joy.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://iqu.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uca.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uiu.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://spb.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uat.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zob.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bcq.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lhl.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bfh.xinyue.icu

================================================================================
来源：http://hrp.shuidangran.top

J. 日期与时间
来源：http://hlx.shanyushiyangtech.top

================================================================================
来源：http://oqa.nanxinkj.top

[J01] 获取当前时间
来源：http://wzm.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hnw.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tjl.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://fun.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://imo.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wmb.yuxming.cn

Go:   time.Now()
来源：http://gqb.jyoumei.cn

Ruby: Time.now
来源：http://uzk.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yar.yuxming.cn

[J02] 格式化输出
来源：http://sfc.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lls.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dln.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ieu.sxryk.cn

TS:   d.toISOString()
来源：http://pks.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sfy.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://exn.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfe.ivvv.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rog.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://nuj.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xck.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tjp.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://igw.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://sxg.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ywn.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ifg.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://zlf.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://stw.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://ayj.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aen.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wav.yongpay.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kyv.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wcf.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ppn.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://djw.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qar.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fqe.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://cxj.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://bse.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ipr.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahb.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bgv.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://lgl.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aib.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://eel.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://zvh.sufxvd.cn

[J06] 计算两时间之差
来源：http://etk.316326.xyz

Py:   (end - start).total_seconds()
来源：http://hkc.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://slh.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://etx.jiagoushi.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vtr.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://caf.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://vri.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://hhk.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://kkc.jlsjyb.cn


<!-- 参考信息 -->