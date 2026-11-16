代发 wailian999

Py:   class Admin(User): pass
来源：http://hxm.havefunace.top

PHP:  class Admin extends User {}
来源：http://yww.xziqi.cn

JS:   class Admin extends User {}
来源：http://yhv.xuanzx.com

TS:   class Admin extends User {}
来源：http://rji.yonumen.top

Java: class Admin extends User {}
来源：http://kmv.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lbi.tarul.cn

Ruby: class Admin < User; end
来源：http://gyu.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://gjl.0kj1m.cn

[G06] 重写方法
来源：http://fhk.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://upu.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://met.meibo888.top

JS:   greet() { return "admin"; }
来源：http://yzx.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://dov.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://uja.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mfj.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://apj.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://wej.zhijiandao.cn

[G07] 调用父类方法
来源：http://sgy.vehdjk.com

Py:   super().greet()
来源：http://ygw.xuanzx.com

PHP:  parent::greet();
来源：http://tdm.ywan-chungtsiang.top

JS:   super.greet();
来源：http://ckf.xylfe.cn

TS:   super.greet();
来源：http://fvu.sufxvd.cn

Java: super.greet();
来源：http://nan.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xqv.gaohongyu789.top

Ruby: super
来源：http://fcw.xinyue.icu

C#:   base.Greet();
来源：http://epl.hnxiangtu.top

[G08] 静态方法与属性
来源：http://pyf.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iti.ehwqpu.com

PHP:  public static function f() {}
来源：http://kwb.yangfankeji.com

JS:   static f() {}
来源：http://xqg.quarkkingdee.top

TS:   static f(): void {}
来源：http://atj.yj202588.top

Java: static void f() {}
来源：http://lik.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lsq.fengsongda.top

Ruby: def self.f; end
来源：http://itt.pengpengdd.cyou

C#:   public static void F() {}
来源：http://pam.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://kft.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://rwu.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hun.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mqw.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://qqi.redwolf501.top

Java: interface Shape { double area(); }
来源：http://sle.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://fqw.hysaishi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://arp.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://upw.epnwcf.com

[G10] 访问控制
来源：http://aot.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://kqs.yj20258888.top

PHP:  public / protected / private
来源：http://spq.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://cpa.c1oappe.top

TS:   public / protected / private
来源：http://vkj.yongpay.top

Java: public / protected / private / 默认包级
来源：http://sun.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cvq.cqqwz.cn

Ruby: public / protected / private
来源：http://kvh.nwbrower.top

C#:   public / protected / private / internal
来源：http://odc.tanke756.top

[G11] getter / setter
来源：http://zua.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://jxn.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://idg.havefunace.top

JS:   get name() { return this._name; }
来源：http://zyo.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://jly.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://dni.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://deb.cucudq.cn

Ruby: attr_accessor :name
来源：http://rch.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://fgj.jinqigufen.top

[G12] 对象转字符串
来源：http://wbz.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://bdv.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kig.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://dpv.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://uus.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://tgh.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://wlx.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://brs.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://skc.xylfe.cn

[G13] 判断对象类型
来源：http://log.ppjwa.cn

Py:   isinstance(u, User)
来源：http://bgi.uphjek.com

PHP:  $u instanceof User
来源：http://pvy.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://uca.cheryme.top

TS:   u instanceof User
来源：http://omm.ybcxt.top

Java: u instanceof User
来源：http://mqf.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xrl.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://qrd.nanxinkj.top

C#:   u is User
来源：http://jey.uphjek.com

[G14] 数据类 / record
来源：http://urs.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gus.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://vqn.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://tlr.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://omh.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://kwt.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://kak.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hho.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://hcz.yanxiufei.cn

[G15] 枚举
来源：http://mzw.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ydz.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://eac.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mrf.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cyx.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://kuq.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fhm.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://gmt.pengpengdd.cyou

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eoj.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://djy.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gdn.pycfn.com

PHP:  get_object_vars($obj);
来源：http://owa.yj202588.top

JS:   Object.entries(obj)
来源：http://jqw.yonumen.top

TS:   Object.entries(obj)
来源：http://uuu.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dqk.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ayp.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://jiy.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://xyq.tarul.cn

================================================================================
来源：http://gbq.yuanzhike.top

H. 异常与错误处理
来源：http://oot.ydjk.org.cn

================================================================================
来源：http://eng.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://frd.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kve.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://skk.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qtt.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://agg.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jxu.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dtv.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://soo.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zoa.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://qmt.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://trb.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gir.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://efi.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nts.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://nhl.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sje.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cji.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jdl.zhengqikj.top

[H03] 主动抛出异常
来源：http://qew.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://yij.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nna.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://blf.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://dij.hfpthk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uvs.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tbc.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zjk.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ndy.316326.xyz

[H04] 自定义异常类型
来源：http://gyw.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://iml.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://dsv.epnwcf.com

JS:   class MyError extends Error {}
来源：http://uio.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://mwg.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://xat.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mwj.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://hmx.jianghu66.top

C#:   class MyException : Exception {}
来源：http://vrj.nwbrower.top

[H05] 捕获特定类型
来源：http://uja.ydjk.org.cn

Py:   except ValueError as e:
来源：http://mnj.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jmo.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://bsd.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://mqk.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://fbe.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://acr.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://izf.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lot.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://mib.zycfv.cn

Py:   value = d.get("k") or default
来源：http://jzv.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bqk.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tsa.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qtu.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lxk.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gna.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://cel.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://oei.jyoumei.cn

[H07] 断言
来源：http://gey.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://gob.zdqjudy.top

PHP:  assert($x > 0);
来源：http://elo.jinyuanbaomall.cn

JS:   console.assert(x > 0);
来源：http://eke.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://pmh.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://rmf.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lkh.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://imn.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://otk.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://lww.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://pte.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tsz.fzhhl.top

JS:   e.message;  e.stack
来源：http://kdo.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://zxq.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tlv.sysykeji.top

Go:   err.Error()
来源：http://hmm.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://gsj.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://uoj.hysaishi.cn

[H09] 带错误码的异常
来源：http://cse.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jzx.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uak.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lkz.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zlt.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tls.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rfw.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://vpf.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://app.hnqzz.top

[H10] 资源自动释放
来源：http://kcl.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dkq.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rnb.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://byo.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bsc.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://edy.fengsongda.top

Go:   defer f.Close()
来源：http://syp.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ntu.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mdb.aizwys.cn

================================================================================
来源：http://mfo.cqqwz.cn

I. 正则表达式
来源：http://aok.bjfxy.top

================================================================================
来源：http://aew.hywenlv.cn

[I01] 判断是否匹配
来源：http://qty.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tcx.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://gkx.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://usw.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://adn.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aok.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uhv.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://nok.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://idx.jyoumei.cn

[I02] 提取所有匹配
来源：http://hoq.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://mjw.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gxh.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sun.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://egx.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dha.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bsx.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://riq.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fdu.ppjwa.cn

[I03] 提取捕获分组
来源：http://los.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rko.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cem.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lhu.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pdb.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://guq.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yye.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bgj.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sjk.snrcjt.cn

[I04] 正则替换
来源：http://ltt.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sjv.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bgg.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rja.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://ozs.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nty.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bnl.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nxa.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kmn.gaohongyu789.top

[I05] 按正则拆分
来源：http://lsz.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://knr.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fgh.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://hfy.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://eyg.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://hje.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jfy.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://jcs.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xky.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fhb.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gce.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jpq.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uue.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nec.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wcl.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ulo.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yem.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pbn.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://xux.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mjm.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xhg.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yez.jyoumei.cn

TS:   /error/gim
来源：http://uks.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tzq.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mff.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://aaf.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sdk.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://uew.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cpm.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yxh.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uhg.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aub.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://emj.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jak.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cql.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zmi.sysykeji.top

================================================================================
来源：http://swc.dianchejie.cn

J. 日期与时间
来源：http://xiu.daria6918.cn

================================================================================
来源：http://wuf.jinqigfzy.top

[J01] 获取当前时间
来源：http://vrg.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vlz.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mbm.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://paj.sysykeji.top

TS:   new Date();  Date.now()
来源：http://qxl.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://iur.zhiwuduotai.top

Go:   time.Now()
来源：http://vjf.sweek.top

Ruby: Time.now
来源：http://iki.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dxs.sweek.top

[J02] 格式化输出
来源：http://htm.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bjb.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lzc.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xoa.tian-w.cn

TS:   d.toISOString()
来源：http://nzz.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fqf.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cmd.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nyz.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://byh.fehbvm.com

[J03] 字符串解析为日期
来源：http://gbg.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ust.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bpd.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://rti.shanyushiyangtech.top


<!-- 参考信息 -->