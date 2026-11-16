代发 wailian999

Java: class Admin extends User {}
来源：http://yyr.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qih.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://xlt.zhengqikj.top

C#:   class Admin : User {}
来源：http://wfe.ehwqpu.com

[G06] 重写方法
来源：http://ckt.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://lsf.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://nny.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://ogx.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://vcf.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://huq.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://neg.yj20258.top

Ruby: def greet; "admin"; end
来源：http://kbi.vqdsnc.cn

C#:   public override string Greet() => "admin";
来源：http://wdo.chenjidiqi.icu

[G07] 调用父类方法
来源：http://azc.fktsv.cn

Py:   super().greet()
来源：http://gmx.xziqi.cn

PHP:  parent::greet();
来源：http://ubw.ppjwa.cn

JS:   super.greet();
来源：http://ntn.hnxiangtu.top

TS:   super.greet();
来源：http://bxa.hnqzz.top

Java: super.greet();
来源：http://xcs.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lsy.guannengcc.top

Ruby: super
来源：http://onv.yvedp.cn

C#:   base.Greet();
来源：http://tml.c1oappe.top

[G08] 静态方法与属性
来源：http://tsz.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hsp.daria6918.cn

PHP:  public static function f() {}
来源：http://jqp.shanyushiyangtech.top

JS:   static f() {}
来源：http://aeb.aizwys.cn

TS:   static f(): void {}
来源：http://lmh.zhengqikj.top

Java: static void f() {}
来源：http://qmn.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xsq.pengpengdd.cyou

Ruby: def self.f; end
来源：http://puf.hongshengwenyu.top

C#:   public static void F() {}
来源：http://ply.fengsongda.top

[G09] 接口 / 抽象类
来源：http://zhu.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://tkc.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://klp.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://rup.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://nhy.fktsv.cn

Java: interface Shape { double area(); }
来源：http://qqy.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://ker.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ign.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://nif.daxiang520.top

[G10] 访问控制
来源：http://hcc.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://jgz.fzhhl.top

PHP:  public / protected / private
来源：http://zqq.sweek.top

JS:   #private 字段；其余公开
来源：http://eql.hongshengwenyu.top

TS:   public / protected / private
来源：http://vgf.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://rdf.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kdh.zhongyouzk.top

Ruby: public / protected / private
来源：http://mzl.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://fpd.fehbvm.com

[G11] getter / setter
来源：http://ala.iojbl.cn

Py:   @property 与 @x.setter
来源：http://nct.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mis.fktsv.cn

JS:   get name() { return this._name; }
来源：http://dui.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://tfu.0kj1m.cn

Java: public String getName() { return name; }
来源：http://yrt.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://dch.uphjek.com

Ruby: attr_accessor :name
来源：http://fjb.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://mdz.bjfxy.top

[G12] 对象转字符串
来源：http://ouu.yj20258.top

Py:   def __str__(self): return self.name
来源：http://vxu.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dmg.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://sjt.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://wth.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://gar.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://uak.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://dze.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://svx.chenlongwang.top

[G13] 判断对象类型
来源：http://kwq.ehwqpu.com

Py:   isinstance(u, User)
来源：http://jax.yueranfly.top

PHP:  $u instanceof User
来源：http://svu.ivvv.top

JS:   u instanceof User
来源：http://tlm.yj202588.top

TS:   u instanceof User
来源：http://vrb.ppjwa.cn

Java: u instanceof User
来源：http://wmu.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rxm.pycfn.com

Ruby: u.is_a?(User)
来源：http://aln.yj20258.top

C#:   u is User
来源：http://ful.meibo888.top

[G14] 数据类 / record
来源：http://veh.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xtb.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://szw.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://xmp.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://kjx.haohaochexian.top

Java: record User(String name, int age) {}
来源：http://tku.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://yxs.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eyh.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://mqy.ivvv.top

[G15] 枚举
来源：http://wfb.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ugk.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bfv.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vep.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pyj.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://jea.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dus.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://axf.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bqj.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://blr.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yuv.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://gdt.snrcjt.cn

JS:   Object.entries(obj)
来源：http://ddd.vehdjk.com

TS:   Object.entries(obj)
来源：http://sgd.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sbn.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qub.wangdashe.top

Ruby: obj.instance_variables
来源：http://dqy.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://wlf.epnwcf.com

================================================================================
来源：http://upy.epnwcf.com

H. 异常与错误处理
来源：http://jnv.guowangkeji.top

================================================================================
来源：http://dab.gogol.net.cn

[H01] try / catch 基础
来源：http://soc.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://udm.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ksm.nanxinkj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zgp.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ntk.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mtd.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://utq.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://clc.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lxx.cucudq.cn

[H02] finally / ensure 收尾
来源：http://jbt.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://suv.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ibl.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://syo.shangyingyoupin.top

TS:   try { f(); } finally { cleanup(); }
来源：http://znp.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://tbu.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ltf.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lpk.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://omf.hfpthk.cn

[H03] 主动抛出异常
来源：http://uqt.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://gwl.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xqk.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://awk.yj202588.top

TS:   throw new Error("错误信息");
来源：http://fzw.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sut.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zwr.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fzh.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://owl.hnxiangtu.top

[H04] 自定义异常类型
来源：http://jst.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://liw.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nqy.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://hmn.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://jmn.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://jvk.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pog.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://ios.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://mam.quarkkingdee.top

[H05] 捕获特定类型
来源：http://sse.gogol.net.cn

Py:   except ValueError as e:
来源：http://fuf.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jef.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://mcb.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://igy.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://bdn.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://npj.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://wtq.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fii.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://brh.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://vqz.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gmt.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://fjo.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ldw.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xer.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://xco.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://lmp.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://fbw.yj20258.top

[H07] 断言
来源：http://lfx.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://zxf.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://cvk.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://oqx.tian-w.cn

TS:   console.assert(x > 0);
来源：http://gtv.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://bhw.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wey.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://plw.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://wly.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://ykt.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://afd.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://drn.hysaishi.cn

JS:   e.message;  e.stack
来源：http://cot.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lja.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sjo.guannengcc.top

Go:   err.Error()
来源：http://ypj.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://kof.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://fjv.wangdashe.top

[H09] 带错误码的异常
来源：http://vfb.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dpu.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ulk.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://znc.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qnn.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ldr.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ohj.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://akh.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zap.andypj.xyz

[H10] 资源自动释放
来源：http://gps.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://axe.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://svz.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://whw.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pmv.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://reb.yfazqb.com

Go:   defer f.Close()
来源：http://eny.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dew.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lyc.mhx1999.top

================================================================================
来源：http://zsu.vehdjk.com

I. 正则表达式
来源：http://vfv.jinghuilouyu.cn

================================================================================
来源：http://xls.gaohongyu789.top

[I01] 判断是否匹配
来源：http://ltj.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ito.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nok.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://xfj.ivvv.top

TS:   /\d+/.test(s)
来源：http://adl.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fnu.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oix.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://yvp.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jhk.yj20258888.top

[I02] 提取所有匹配
来源：http://pnm.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://eqo.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eho.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pgz.uphjek.com

TS:   s.match(/\d+/g)
来源：http://bix.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xoa.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jea.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://ock.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qym.zhoulong.xyz

[I03] 提取捕获分组
来源：http://qcp.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zkv.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hrx.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lta.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ezw.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jvd.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jil.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kqm.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://spi.jinqigufen.top

[I04] 正则替换
来源：http://atg.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ogy.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sfs.redwolf501.top

JS:   s.replace(/\d+/g, "#")
来源：http://hfe.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://dng.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://bwq.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vuu.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kba.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://myk.yj20258.top

[I05] 按正则拆分
来源：http://jgx.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xkf.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ltl.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://tks.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://ypn.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://oid.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ofc.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://nwi.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qnp.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rgd.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://djx.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vnc.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xwv.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kyk.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cst.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nig.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cmz.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://efa.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://blg.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sex.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://imd.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bvh.jqgfzy.top

TS:   /error/gim
来源：http://sqg.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vtg.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tlr.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://ssk.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nfv.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://omz.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xyp.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iwo.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nom.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtt.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xqm.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fcn.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lqx.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://agy.xuanzx.com

================================================================================
来源：http://uno.mhx1999.top

J. 日期与时间
来源：http://sst.daria6918.cn

================================================================================
来源：http://vxr.haohaochexian.top

[J01] 获取当前时间
来源：http://yds.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://jnu.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ysf.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://smg.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://qsr.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://knc.cdnleiting.top

Go:   time.Now()
来源：http://vkc.chenlongwang.top

Ruby: Time.now
来源：http://kqb.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fii.daxiang520.top

[J02] 格式化输出
来源：http://fvd.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dvz.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xui.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lnd.gogol.net.cn

TS:   d.toISOString()
来源：http://edz.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mgs.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aqi.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzx.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fmt.fzhhl.top

[J03] 字符串解析为日期
来源：http://jzm.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pqz.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yrl.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://gpn.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://lcq.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://hjd.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hcw.guowangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://wfi.316326.xyz


<!-- 参考信息 -->