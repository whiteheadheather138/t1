代发 wailian999

Py:   class Admin(User): pass
来源：http://cez.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://bkl.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://lvv.tanke756.top

TS:   class Admin extends User {}
来源：http://mel.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://pxd.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qkz.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://uvx.vehdjk.com

C#:   class Admin : User {}
来源：http://lja.jinghuilouyu.cn

[G06] 重写方法
来源：http://gbi.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://upg.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uhu.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://hxx.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://cbt.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://krb.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ice.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://rok.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://tau.tarul.cn

[G07] 调用父类方法
来源：http://unr.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://cwr.yuxming.cn

PHP:  parent::greet();
来源：http://dtk.ctjpmb.com

JS:   super.greet();
来源：http://gxp.yonumen.top

TS:   super.greet();
来源：http://xuf.hammf.cn

Java: super.greet();
来源：http://ddf.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ycp.yangfankeji.com

Ruby: super
来源：http://fpx.feifeiyinyue.top

C#:   base.Greet();
来源：http://pgh.yj20258888.top

[G08] 静态方法与属性
来源：http://brr.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sqz.yj20258888.top

PHP:  public static function f() {}
来源：http://dra.mhx1999.top

JS:   static f() {}
来源：http://mwr.svipenyu.cn

TS:   static f(): void {}
来源：http://glf.jiagoushi.top

Java: static void f() {}
来源：http://jdy.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xmo.yvedp.cn

Ruby: def self.f; end
来源：http://jxn.cdnleiting.top

C#:   public static void F() {}
来源：http://klk.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://eam.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://upa.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://dea.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lon.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://ryf.bjfxy.top

Java: interface Shape { double area(); }
来源：http://dur.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://fed.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dzd.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://tui.bbcook.cn

[G10] 访问控制
来源：http://byx.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://zjy.jinqigfzy.top

PHP:  public / protected / private
来源：http://fos.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://hea.wangshuangyany.cn

TS:   public / protected / private
来源：http://cqb.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://fqs.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://fvq.chenjidiqi.icu

Ruby: public / protected / private
来源：http://tdg.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://tok.sweek.top

[G11] getter / setter
来源：http://fsk.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://oxa.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lwl.wangdashe.top

JS:   get name() { return this._name; }
来源：http://gak.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://wqs.ybcxt.top

Java: public String getName() { return name; }
来源：http://vtc.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://isp.xuanzx.com

Ruby: attr_accessor :name
来源：http://nln.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://pvd.hfpthk.cn

[G12] 对象转字符串
来源：http://utt.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://qai.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://brf.hammf.cn

JS:   toString() { return this.name; }
来源：http://ezj.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://xqk.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://grr.pycfn.com

Go:   func (u User) String() string { return u.Name }
来源：http://rao.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://vqs.ivvv.top

C#:   public override string ToString() => Name;
来源：http://hfs.guowangkeji.top

[G13] 判断对象类型
来源：http://abg.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://kqf.birdmap.top

PHP:  $u instanceof User
来源：http://wcd.wangshuangyany.cn

JS:   u instanceof User
来源：http://gkk.bjfxy.top

TS:   u instanceof User
来源：http://kil.shanyushiyangtech.top

Java: u instanceof User
来源：http://txx.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://zdk.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://iuu.wangdashe.top

C#:   u is User
来源：http://shx.ppjwa.cn

[G14] 数据类 / record
来源：http://tvx.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://itb.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://flz.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://knk.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://gih.xylfe.cn

Java: record User(String name, int age) {}
来源：http://xdd.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://rks.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rgy.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://anj.sufxvd.cn

[G15] 枚举
来源：http://pvq.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ptx.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tzt.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mpr.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://znt.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://ova.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://epf.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://ksa.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xms.316326.xyz

[G16] 对象转数组 / 字典
来源：http://ypm.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gbc.zhaomingkeji.xyz

PHP:  get_object_vars($obj);
来源：http://jib.tian-w.cn

JS:   Object.entries(obj)
来源：http://gnb.ehwqpu.com

TS:   Object.entries(obj)
来源：http://nda.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pjj.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://cin.tarul.cn

Ruby: obj.instance_variables
来源：http://frz.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://wwe.ppjwa.cn

================================================================================
来源：http://sbf.shuidangran.top

H. 异常与错误处理
来源：http://kpe.nanxinkj.top

================================================================================
来源：http://uac.redwolf501.top

[H01] try / catch 基础
来源：http://ijr.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://llq.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ngm.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vej.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rfu.52xcode.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qby.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dan.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hal.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://swv.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://bku.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://tsw.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://onq.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iss.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://bpu.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://dww.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://cfw.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ama.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pam.smart0.xyz

[H03] 主动抛出异常
来源：http://tbz.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://tmu.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cyb.tanke756.top

JS:   throw new Error("错误信息");
来源：http://nxa.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://jqv.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mdq.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xvs.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qop.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://sus.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://oju.tanke756.top

Py:   class MyError(Exception): pass
来源：http://ndu.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://xey.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://lku.yj202588.top

TS:   class MyError extends Error {}
来源：http://min.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://qra.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nll.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://qbi.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://rel.zhijiandao.cn

[H05] 捕获特定类型
来源：http://rmg.bbcook.cn

Py:   except ValueError as e:
来源：http://uhh.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://snt.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://kpd.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://eyp.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://red.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lqt.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://uho.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zrb.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://vae.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://tez.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://jmp.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://gmx.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tra.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ubs.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ggu.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://jff.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://lwl.jinqigfzy.top

[H07] 断言
来源：http://iqd.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://alg.tarul.cn

PHP:  assert($x > 0);
来源：http://ede.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://gtp.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://mdo.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://mzs.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lhm.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://tmh.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://bau.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://oop.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://kep.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://swk.c1oappe.top

JS:   e.message;  e.stack
来源：http://uoq.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pqj.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jqf.zhengqikj.top

Go:   err.Error()
来源：http://kpi.sweek.top

Ruby: e.message;  e.backtrace
来源：http://wof.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://auy.zdbjq.cn

[H09] 带错误码的异常
来源：http://jwa.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ina.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hum.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zqj.0kj1m.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zir.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://svl.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mtr.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://wet.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lqb.shzxlz.cn

[H10] 资源自动释放
来源：http://epn.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fxg.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hpj.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dwd.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://slj.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ver.dashuyun.cn

Go:   defer f.Close()
来源：http://ytk.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ncn.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gro.ivvv.top

================================================================================
来源：http://qfn.sysykeji.top

I. 正则表达式
来源：http://enc.sweek.top

================================================================================
来源：http://qia.birdmap.top

[I01] 判断是否匹配
来源：http://wqe.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hpz.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://hua.52xcode.cn

JS:   /\d+/.test(s)
来源：http://eqj.fzhhl.top

TS:   /\d+/.test(s)
来源：http://dio.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jei.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wij.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://xlf.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yjc.gogol.net.cn

[I02] 提取所有匹配
来源：http://mrh.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://vds.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ehj.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yym.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://ujy.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wim.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jsv.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://bpg.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://byv.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://ctp.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zdu.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://csl.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yio.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uef.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cpr.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wpd.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://swo.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kdo.yuxming.cn

[I04] 正则替换
来源：http://hfa.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://pba.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://moc.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://czz.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://aap.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://wgb.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pas.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://btg.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dnp.tanke756.top

[I05] 按正则拆分
来源：http://sbg.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yfk.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://glm.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://wbd.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://tcp.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://rsa.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eji.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://xkm.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ukt.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vwe.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kha.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://alo.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ynj.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://myh.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rol.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://avu.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ufe.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://omw.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://ani.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ldw.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kuj.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iuk.redwolf501.top

TS:   /error/gim
来源：http://qvu.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://frg.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lhq.cheryme.top

Ruby: s.scan(/error/i)
来源：http://nlu.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://brt.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://pzm.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://luw.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fuc.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rxq.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfm.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rhs.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bwz.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sek.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zgm.52xcode.cn

================================================================================
来源：http://tit.hnxiangtu.top

J. 日期与时间
来源：http://iwl.zdbjq.cn

================================================================================
来源：http://jrb.jqgufenzy.top

[J01] 获取当前时间
来源：http://miu.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cfv.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fkj.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://hqf.xuanzx.com

TS:   new Date();  Date.now()
来源：http://anb.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fvq.zhijiandao.cn

Go:   time.Now()
来源：http://lak.yongpay.top

Ruby: Time.now
来源：http://zdg.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ugb.yangfankeji.com

[J02] 格式化输出
来源：http://piz.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rsp.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ktc.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://coy.jlsjyb.cn

TS:   d.toISOString()
来源：http://qti.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oej.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://okd.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qui.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zjc.gotoacloud.top

[J03] 字符串解析为日期
来源：http://afk.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uhf.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vao.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://gcq.aizwys.cn


<!-- 参考信息 -->