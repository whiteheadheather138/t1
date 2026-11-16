代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://xca.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://xoz.cashguo.top

TS:   greet(): string { return this.name; }
来源：http://xrs.hysaishi.cn

Java: String greet() { return name; }
来源：http://cap.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mzg.guannengcc.top

Ruby: def greet; @name; end
来源：http://hjw.yj20258888.top

C#:   public string Greet() => Name;
来源：http://wgi.epnwcf.com

[G05] 继承
来源：http://xct.sweek.top

Py:   class Admin(User): pass
来源：http://wqh.zycfv.cn

PHP:  class Admin extends User {}
来源：http://lav.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://xtz.cqqwz.cn

TS:   class Admin extends User {}
来源：http://cjb.zhengqikj.top

Java: class Admin extends User {}
来源：http://opl.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bqs.zhengqikj.top

Ruby: class Admin < User; end
来源：http://yel.sufxvd.cn

C#:   class Admin : User {}
来源：http://yus.hcnkem.com

[G06] 重写方法
来源：http://npx.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://ope.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zjr.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://qwn.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://uiz.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://avo.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://php.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://dwr.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://lnf.aizwys.cn

[G07] 调用父类方法
来源：http://nop.epnwcf.com

Py:   super().greet()
来源：http://nqq.jlsjyb.cn

PHP:  parent::greet();
来源：http://njx.jinghuilouyu.cn

JS:   super.greet();
来源：http://noq.aibaodan.cn

TS:   super.greet();
来源：http://aue.redwolf501.top

Java: super.greet();
来源：http://zcg.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aif.hnxiangtu.top

Ruby: super
来源：http://wxf.52xcode.cn

C#:   base.Greet();
来源：http://jck.sysykeji.top

[G08] 静态方法与属性
来源：http://ntd.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yzr.jinqigfzy.top

PHP:  public static function f() {}
来源：http://uqw.tianlin.xyz

JS:   static f() {}
来源：http://xux.ydzc1.top

TS:   static f(): void {}
来源：http://ggs.ybcxt.top

Java: static void f() {}
来源：http://qso.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eaz.wangshuangyany.cn

Ruby: def self.f; end
来源：http://nbc.birdmap.top

C#:   public static void F() {}
来源：http://yvm.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://rnd.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://rjf.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bpb.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fkv.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://gko.shuidangran.top

Java: interface Shape { double area(); }
来源：http://zem.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://yix.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nrv.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://fja.yonumen.top

[G10] 访问控制
来源：http://icl.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://fdj.zdqjudy.top

PHP:  public / protected / private
来源：http://qdu.vehdjk.com

JS:   #private 字段；其余公开
来源：http://lmz.zhixingplan.top

TS:   public / protected / private
来源：http://gxo.uphjek.com

Java: public / protected / private / 默认包级
来源：http://elv.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qry.nanxinkj.top

Ruby: public / protected / private
来源：http://dep.sweek.top

C#:   public / protected / private / internal
来源：http://ugi.xuanzx.com

[G11] getter / setter
来源：http://mgg.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://ctv.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fui.epnwcf.com

JS:   get name() { return this._name; }
来源：http://mnn.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://kls.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://ufs.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://dyo.haohaochexian.top

Ruby: attr_accessor :name
来源：http://hzy.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://kkg.guannengcc.top

[G12] 对象转字符串
来源：http://jvi.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://nxb.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://poh.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://xrw.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://lky.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://vbv.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jhy.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://yen.hammf.cn

C#:   public override string ToString() => Name;
来源：http://lpx.tian-w.cn

[G13] 判断对象类型
来源：http://nfl.hywenlv.cn

Py:   isinstance(u, User)
来源：http://yqw.iojbl.cn

PHP:  $u instanceof User
来源：http://goz.jqgfzy.top

JS:   u instanceof User
来源：http://ejy.jyoumei.cn

TS:   u instanceof User
来源：http://jav.haohaochexian.top

Java: u instanceof User
来源：http://bbk.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://apm.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://eqg.chenzaomai.com

C#:   u is User
来源：http://pwl.yanxiufei.cn

[G14] 数据类 / record
来源：http://sav.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vie.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://zah.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://kid.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://fsb.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://iue.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://ycx.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uvl.yongpay.top

C#:   record User(string Name, int Age);
来源：http://kvu.wangdashe.top

[G15] 枚举
来源：http://qdt.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mxt.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hdn.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tjn.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hje.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://btl.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dpq.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://rok.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dni.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://tzv.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gvp.yj20258.top

PHP:  get_object_vars($obj);
来源：http://duf.yueranfly.top

JS:   Object.entries(obj)
来源：http://kmf.jianghu66.top

TS:   Object.entries(obj)
来源：http://efz.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mrg.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://owy.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://mmb.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://nhp.yuanzhike.top

================================================================================
来源：http://qrv.jlsjyb.cn

H. 异常与错误处理
来源：http://irn.chenzaomai.com

================================================================================
来源：http://ubk.cheryme.top

[H01] try / catch 基础
来源：http://xyt.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fim.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://waq.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mxy.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nnm.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aup.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://clp.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ymf.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bwf.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://hel.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hbx.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tfw.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://khb.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zuk.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://nrn.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://amq.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zcn.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yve.yj202588.top

[H03] 主动抛出异常
来源：http://umk.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://jhb.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://omt.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://rdv.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://dqf.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lxt.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lsu.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://cwe.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zpv.cqqwz.cn

[H04] 自定义异常类型
来源：http://drh.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://fwp.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://jaw.redwolf501.top

JS:   class MyError extends Error {}
来源：http://fyh.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://tbi.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://xcc.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vto.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://jcw.bjfxy.top

C#:   class MyException : Exception {}
来源：http://zbl.ppjwa.cn

[H05] 捕获特定类型
来源：http://zhi.svipenyu.cn

Py:   except ValueError as e:
来源：http://qna.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oao.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://imn.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://tbb.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://dhe.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ofa.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://vlz.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mjl.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://fey.fzhhl.top

Py:   value = d.get("k") or default
来源：http://asx.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xlz.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://mna.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://vda.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cyj.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cbt.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://fyo.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://pma.yuxming.cn

[H07] 断言
来源：http://txr.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://evc.ehwqpu.com

PHP:  assert($x > 0);
来源：http://xrv.xylfe.cn

JS:   console.assert(x > 0);
来源：http://oby.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://quf.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://puw.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fdq.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://kzv.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://pif.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://pab.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://wud.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xwg.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://jac.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fub.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ltl.ywan-chungtsiang.top

Go:   err.Error()
来源：http://oqx.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://mvs.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://cip.nanxuanxn.top

[H09] 带错误码的异常
来源：http://ctf.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aia.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://xrl.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sms.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jot.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tzh.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://knb.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://kzv.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rvg.jinqigfzy.top

[H10] 资源自动释放
来源：http://oqk.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://klm.epnwcf.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fgn.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qnx.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bxj.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://krr.yuxming.cn

Go:   defer f.Close()
来源：http://kfz.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zpf.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iug.hongshengwenyu.top

================================================================================
来源：http://bwz.pengpengdd.cyou

I. 正则表达式
来源：http://wwl.316326.xyz

================================================================================
来源：http://wyf.jiagoushi.top

[I01] 判断是否匹配
来源：http://jnt.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yhn.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jlr.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://zcg.havefunace.top

TS:   /\d+/.test(s)
来源：http://lhz.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rit.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://agx.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://mnp.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vto.gaohongyu789.top

[I02] 提取所有匹配
来源：http://ilu.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://skr.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hej.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pkq.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://ryb.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dtb.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jdi.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://uql.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fjs.yvedp.cn

[I03] 提取捕获分组
来源：http://axj.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bdl.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qwb.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ucu.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pga.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bcj.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mdx.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jjd.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://amf.sweek.top

[I04] 正则替换
来源：http://qed.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hjq.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ghf.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://ada.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rgc.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ewp.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fos.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://fgi.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://frj.fzhhl.top

[I05] 按正则拆分
来源：http://vly.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xyn.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tbc.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://acs.yj20258.top

TS:   s.split(/\s*,\s*/)
来源：http://ygt.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://wxt.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dzy.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://txu.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://crx.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ibj.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sxs.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hyb.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvd.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zgi.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wcw.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vbx.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yxc.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dqc.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://btx.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uem.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://atx.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://swx.chenlongwang.top

TS:   /error/gim
来源：http://xne.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://did.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://npd.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://dto.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://geh.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://tpm.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gbd.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hai.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tjk.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bcu.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://thm.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bni.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vjr.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pvt.xingfuxueyuan.xyz

================================================================================
来源：http://aur.guowangkeji.top

J. 日期与时间
来源：http://jxd.ydjk.org.cn

================================================================================
来源：http://bbp.pycfn.com

[J01] 获取当前时间
来源：http://xvz.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ija.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jkj.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://ggx.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://rdo.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://weq.chenlongwang.top

Go:   time.Now()
来源：http://mjx.jqgufenzy.top

Ruby: Time.now
来源：http://bts.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tbl.yj202588.top

[J02] 格式化输出
来源：http://znb.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://epz.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rvp.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://akn.hammf.cn

TS:   d.toISOString()
来源：http://tpi.0kj1m.cn


<!-- 参考信息 -->