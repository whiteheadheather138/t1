代发 wailian999

Java: class Admin extends User {}
来源：http://rrj.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fhg.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://csj.andypj.xyz

C#:   class Admin : User {}
来源：http://koq.yangfankeji.com

[G06] 重写方法
来源：http://tpf.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://zkl.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mzp.tarul.cn

JS:   greet() { return "admin"; }
来源：http://xzg.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://inq.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://ugw.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vrr.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://ysx.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://ori.vqdsnc.cn

[G07] 调用父类方法
来源：http://wkp.shuidangran.top

Py:   super().greet()
来源：http://xst.yangfankeji.com

PHP:  parent::greet();
来源：http://jer.daxiang520.top

JS:   super.greet();
来源：http://vtf.cqqwz.cn

TS:   super.greet();
来源：http://dqu.zhixingplan.top

Java: super.greet();
来源：http://qlx.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://acv.fehbvm.com

Ruby: super
来源：http://yvo.zdqjudy.top

C#:   base.Greet();
来源：http://wwp.smart0.xyz

[G08] 静态方法与属性
来源：http://bbx.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cff.gzhubu.top

PHP:  public static function f() {}
来源：http://hmg.xuanzx.com

JS:   static f() {}
来源：http://kls.ydzc1.top

TS:   static f(): void {}
来源：http://yxs.yfazqb.com

Java: static void f() {}
来源：http://qgu.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://isi.hfpthk.cn

Ruby: def self.f; end
来源：http://sam.zhengqikj.top

C#:   public static void F() {}
来源：http://xpu.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://ukw.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://ikh.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://sll.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://krj.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://zdm.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://uxi.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://dgv.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wji.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://fqt.yuanzhike.top

[G10] 访问控制
来源：http://pvk.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://ueb.jinqigufen.top

PHP:  public / protected / private
来源：http://ekg.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://rqb.gogol.net.cn

TS:   public / protected / private
来源：http://sbp.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://tqh.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fvs.fanxiaobao.xyz

Ruby: public / protected / private
来源：http://jti.hesvh.cn

C#:   public / protected / private / internal
来源：http://mmd.shanyushiyangkeji.top

[G11] getter / setter
来源：http://wfj.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://pbn.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kwl.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://ehu.mhx1999.top

TS:   get name(): string { return this._name; }
来源：http://odl.havefunace.top

Java: public String getName() { return name; }
来源：http://irs.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fqg.yj20258888.top

Ruby: attr_accessor :name
来源：http://lpy.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://gjf.hesvh.cn

[G12] 对象转字符串
来源：http://aei.316326.xyz

Py:   def __str__(self): return self.name
来源：http://dua.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bhm.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://ecg.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://bex.chenzaomai.com

Java: @Override public String toString() { return name; }
来源：http://gme.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://mjt.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://vxf.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://tkl.ydzc1.top

[G13] 判断对象类型
来源：http://fyf.sufxvd.cn

Py:   isinstance(u, User)
来源：http://dkc.yj202588.top

PHP:  $u instanceof User
来源：http://sez.chenjidiqi.icu

JS:   u instanceof User
来源：http://esf.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://lzw.shzxlz.cn

Java: u instanceof User
来源：http://xvw.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://res.yueranfly.top

Ruby: u.is_a?(User)
来源：http://hhm.0kj1m.cn

C#:   u is User
来源：http://wph.c1oappe.top

[G14] 数据类 / record
来源：http://mhk.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wcu.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://bcm.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://utq.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://rox.jianghu66.top

Java: record User(String name, int age) {}
来源：http://flj.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://oft.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://grz.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://egl.zhiwuduotai.top

[G15] 枚举
来源：http://ttl.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pou.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rdi.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bvn.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wje.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://wxg.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pvu.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://xqp.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rka.uphjek.com

[G16] 对象转数组 / 字典
来源：http://mnp.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rhy.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://pcx.yuanzhike.top

JS:   Object.entries(obj)
来源：http://pym.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://qan.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vve.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pbc.sweek.top

Ruby: obj.instance_variables
来源：http://wzw.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://hot.mhx1999.top

================================================================================
来源：http://gbb.quarkkingdee.top

H. 异常与错误处理
来源：http://ymj.pengpengdd.cyou

================================================================================
来源：http://zzs.feifeiyinyue.top

[H01] try / catch 基础
来源：http://gpw.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gix.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hbo.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ajc.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://him.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ska.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nbo.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ebb.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mue.uphjek.com

[H02] finally / ensure 收尾
来源：http://xyz.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ydk.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kmh.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ogt.chenjidiqi.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://aco.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ayw.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://laz.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nyv.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ldx.sjlbkw.cn

[H03] 主动抛出异常
来源：http://cfw.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://jhf.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dic.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://jtz.sweek.top

TS:   throw new Error("错误信息");
来源：http://iua.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nip.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bne.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lts.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://ofl.xinyue.icu

[H04] 自定义异常类型
来源：http://zsr.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://mjn.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://xim.tanke756.top

JS:   class MyError extends Error {}
来源：http://gik.nwbrower.top

TS:   class MyError extends Error {}
来源：http://idw.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://qsp.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gyb.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://vai.wangdashe.top

C#:   class MyException : Exception {}
来源：http://bfp.jqgufenzy.top

[H05] 捕获特定类型
来源：http://skr.andypj.xyz

Py:   except ValueError as e:
来源：http://idv.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qts.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://xjy.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://rtl.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://qtp.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pqu.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://dsz.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jtl.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://acy.aizwys.cn

Py:   value = d.get("k") or default
来源：http://awa.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qvx.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://dzc.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://zza.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cgr.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lvf.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://arb.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://izd.cheryme.top

[H07] 断言
来源：http://dtb.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://kzu.hfpthk.cn

PHP:  assert($x > 0);
来源：http://zck.fehbvm.com

JS:   console.assert(x > 0);
来源：http://spb.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://xih.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://tdk.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tsk.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://tfx.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://mmv.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://lkl.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://eml.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kwd.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://req.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lsr.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://idv.pengpengdd.cyou

Go:   err.Error()
来源：http://txs.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://vgn.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://vxt.zdqjudy.top

[H09] 带错误码的异常
来源：http://tyq.nanxinkj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nnt.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yfh.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pai.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gzr.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://znz.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xrz.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kuy.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kch.jqgufenzy.top

[H10] 资源自动释放
来源：http://zei.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rff.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qkb.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fal.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://exy.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eqf.hywenlv.cn

Go:   defer f.Close()
来源：http://ofw.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vmv.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vqo.jinqigufen.top

================================================================================
来源：http://fbv.shanyushiyangkeji.top

I. 正则表达式
来源：http://wmh.nwbrower.top

================================================================================
来源：http://xgk.9152youxi.cn

[I01] 判断是否匹配
来源：http://cvl.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gqq.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://jqn.andypj.xyz

JS:   /\d+/.test(s)
来源：http://hox.yfazqb.com

TS:   /\d+/.test(s)
来源：http://gia.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fir.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://agg.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://jnb.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zye.nwbrower.top

[I02] 提取所有匹配
来源：http://ecz.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://zni.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://epu.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jcg.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://hbm.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://plx.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dii.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://cqk.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aij.jinqigfzy.top

[I03] 提取捕获分组
来源：http://ned.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://inw.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bil.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybw.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ssq.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kud.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tqi.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://laf.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pdr.ywan-chungtsiang.top

[I04] 正则替换
来源：http://qod.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hrm.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ujk.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://sgk.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://bjl.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://arq.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ajf.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bjo.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ifu.tarul.cn

[I05] 按正则拆分
来源：http://zsr.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oiq.chenjidiqi.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://urw.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://xps.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://sfz.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://ugr.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gro.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://gvu.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://arm.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xeb.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zeu.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ljg.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vhl.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rya.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mmv.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://upo.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ogx.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lvg.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://rtn.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://goh.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wsw.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ybo.cheryme.top

TS:   /error/gim
来源：http://wva.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zrz.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fbs.316326.xyz

Ruby: s.scan(/error/i)
来源：http://fmq.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jlr.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://ixc.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eyy.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mwl.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pup.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gan.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dky.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fhv.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wfg.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eup.xziqi.cn

================================================================================
来源：http://rzt.smart0.xyz

J. 日期与时间
来源：http://uiu.yj202588.top

================================================================================
来源：http://bmn.ydjk.org.cn

[J01] 获取当前时间
来源：http://nni.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ouk.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qdw.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://pfz.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://btx.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://wxv.epnwcf.com

Go:   time.Now()
来源：http://ssf.zycfv.cn

Ruby: Time.now
来源：http://war.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ozv.jqgufenzy.top

[J02] 格式化输出
来源：http://tbo.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uzg.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rhk.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://feu.sweek.top

TS:   d.toISOString()
来源：http://zbk.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pax.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wsm.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://grs.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uzs.zycfv.cn

[J03] 字符串解析为日期
来源：http://bas.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hdy.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dak.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://ouw.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://fto.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://shv.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vvc.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://dls.yuxming.cn


<!-- 参考信息 -->