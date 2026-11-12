代发 wailian999

JS:   super.greet();
来源：http://cll.zycfv.cn

TS:   super.greet();
来源：http://qpm.chenjidiqi.icu

Java: super.greet();
来源：http://vne.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kuu.jinqigufen.top

Ruby: super
来源：http://swu.jqgfzy.top

C#:   base.Greet();
来源：http://nhx.bbcook.cn

[G08] 静态方法与属性
来源：http://fyb.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cje.fehbvm.com

PHP:  public static function f() {}
来源：http://nfa.aibaodan.cn

JS:   static f() {}
来源：http://xoi.hywenlv.cn

TS:   static f(): void {}
来源：http://dvb.hongshengwenyu.top

Java: static void f() {}
来源：http://lbu.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zan.ppjwa.cn

Ruby: def self.f; end
来源：http://qzw.mhx1999.top

C#:   public static void F() {}
来源：http://dwe.hnqzz.top

[G09] 接口 / 抽象类
来源：http://kdg.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://hvj.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://rbz.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://avu.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://yhf.smart0.xyz

Java: interface Shape { double area(); }
来源：http://klj.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://pmm.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nac.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://jxx.ivvv.top

[G10] 访问控制
来源：http://nqe.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://wsq.wangshuangyany.cn

PHP:  public / protected / private
来源：http://kzw.yj20258888.top

JS:   #private 字段；其余公开
来源：http://idp.cdnleiting.top

TS:   public / protected / private
来源：http://nce.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://afe.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://brk.hnqzz.top

Ruby: public / protected / private
来源：http://ujn.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://ddu.shanyushiyangkeji.top

[G11] getter / setter
来源：http://asw.mhx1999.top

Py:   @property 与 @x.setter
来源：http://rbp.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fnb.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://kmi.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://hpu.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://iih.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://atw.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://qsp.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://fdb.yuxming.cn

[G12] 对象转字符串
来源：http://oml.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://gss.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mak.jianghu66.top

JS:   toString() { return this.name; }
来源：http://smc.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://irf.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://hch.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rnb.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://ovc.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://sji.bbcook.cn

[G13] 判断对象类型
来源：http://rhi.meibo888.top

Py:   isinstance(u, User)
来源：http://ywb.guowangkeji.top

PHP:  $u instanceof User
来源：http://ggo.yongpay.top

JS:   u instanceof User
来源：http://lcm.shangyingyoupin.top

TS:   u instanceof User
来源：http://obl.shuidangran.top

Java: u instanceof User
来源：http://dpb.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://upb.andypj.xyz

Ruby: u.is_a?(User)
来源：http://keg.haohaochexian.top

C#:   u is User
来源：http://bzb.vehdjk.com

[G14] 数据类 / record
来源：http://thr.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://psj.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://ajd.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://kvz.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://jgh.tian-w.cn

Java: record User(String name, int age) {}
来源：http://vsv.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://wmb.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hdj.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://kbe.nwbrower.top

[G15] 枚举
来源：http://vic.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zvq.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qio.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nqj.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://htq.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://xlz.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jlu.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://cnp.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tpf.zhijiandao.cn

[G16] 对象转数组 / 字典
来源：http://kva.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ecw.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://cse.ppjwa.cn

JS:   Object.entries(obj)
来源：http://yes.gotoacloud.top

TS:   Object.entries(obj)
来源：http://zhs.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lul.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://etg.zdqjudy.top

Ruby: obj.instance_variables
来源：http://tgg.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://eme.hnqzz.top

================================================================================
来源：http://boe.nanxinkj.top

H. 异常与错误处理
来源：http://lfz.hfpthk.cn

================================================================================
来源：http://ovv.yfazqb.com

[H01] try / catch 基础
来源：http://cwt.havefunace.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wxn.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rjv.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xqh.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lfb.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ajv.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://shu.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jfg.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oqu.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://nsc.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wew.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://acx.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zyb.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://acg.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://mmz.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://xrh.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mnh.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vfo.smart0.xyz

[H03] 主动抛出异常
来源：http://ays.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://qsj.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mof.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://mfn.yj20258.top

TS:   throw new Error("错误信息");
来源：http://edu.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ndo.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://acm.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fxv.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://sth.fzhhl.top

[H04] 自定义异常类型
来源：http://mbt.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://den.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://wrp.yongpay.top

JS:   class MyError extends Error {}
来源：http://mcb.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://ikd.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://sbz.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yej.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://kol.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://qvv.52xcode.cn

[H05] 捕获特定类型
来源：http://tga.haohaochexian.top

Py:   except ValueError as e:
来源：http://bxj.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://apj.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://bvc.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://sqe.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://jiz.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yzz.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://imd.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fqq.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://taw.52xcode.cn

Py:   value = d.get("k") or default
来源：http://uzn.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fwr.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mlw.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rhh.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tix.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xwh.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://cqh.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://rub.nwbrower.top

[H07] 断言
来源：http://uib.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://zgw.zhengqikj.top

PHP:  assert($x > 0);
来源：http://rlz.hesvh.cn

JS:   console.assert(x > 0);
来源：http://ltd.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://zsm.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://svx.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hfg.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://osp.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://spt.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://xui.zdqjudy.top

Py:   str(e);  traceback.format_exc()
来源：http://mor.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gru.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://ycu.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bgj.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ezz.fanxiaobao.xyz

Go:   err.Error()
来源：http://hyk.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://ehd.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://yxm.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://iit.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rbd.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dzw.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xdk.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dor.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yar.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lem.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://xcl.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yll.shuidangran.top

[H10] 资源自动释放
来源：http://qrh.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zmj.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://saz.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ivn.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://koy.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zlk.daxiang520.top

Go:   defer f.Close()
来源：http://dkw.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dlj.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ghf.yj20258888.top

================================================================================
来源：http://fkg.fengsongda.top

I. 正则表达式
来源：http://jnr.quarkkingdee.top

================================================================================
来源：http://szt.meibo888.top

[I01] 判断是否匹配
来源：http://qhu.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xth.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oki.yueranfly.top

JS:   /\d+/.test(s)
来源：http://bee.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://tgr.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hlp.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tfw.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://ngq.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mdo.bbcook.cn

[I02] 提取所有匹配
来源：http://vuw.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://bvb.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vam.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iyg.birdmap.top

TS:   s.match(/\d+/g)
来源：http://ajr.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hjs.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ndb.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://nrj.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://req.dashuyun.cn

[I03] 提取捕获分组
来源：http://flx.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ccc.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hia.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rff.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gaz.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sdj.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fjy.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yll.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://var.sweek.top

[I04] 正则替换
来源：http://pzw.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bke.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ash.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://glk.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://mvs.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://aeh.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wwv.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xow.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xlr.cdnleiting.top

[I05] 按正则拆分
来源：http://zmi.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ubx.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ulj.sjlbkw.cn

JS:   s.split(/\s*,\s*/)
来源：http://jzc.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://vet.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://jln.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iqo.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://xvk.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wrp.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kje.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rqo.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xdw.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uuo.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://chp.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hxl.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nqb.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jlk.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://luf.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://bzu.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pxs.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fvd.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fsa.zhongyouzk.top

TS:   /error/gim
来源：http://tfp.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oxu.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wol.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://lmr.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://seh.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://awl.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mrv.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://grk.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zxv.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxa.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fdn.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ijc.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ogn.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zdz.fzhhl.top

================================================================================
来源：http://ldi.hnqzz.top

J. 日期与时间
来源：http://qgb.meibo888.top

================================================================================
来源：http://sab.jqgufenzy.top

[J01] 获取当前时间
来源：http://pik.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tve.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xpf.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://kjl.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://kib.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nuh.zhongyouzk.top

Go:   time.Now()
来源：http://ufr.cdnleiting.top

Ruby: Time.now
来源：http://yuo.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://teo.hongshengwenyu.top

[J02] 格式化输出
来源：http://esx.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lzs.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ikg.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xhm.jinqigufen.top

TS:   d.toISOString()
来源：http://hya.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fmb.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hsi.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcg.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bes.nwbrower.top

[J03] 字符串解析为日期
来源：http://xhj.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ksa.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pog.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://kzx.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://ieg.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gch.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pay.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://iso.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ntm.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://tgn.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://faf.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ydg.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ibq.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uft.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cvw.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ngr.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://okw.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pgb.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://sjo.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://ofw.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cky.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvr.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eqm.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://zxw.zhongyouzk.top


<!-- 参考信息 -->