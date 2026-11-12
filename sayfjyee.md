代发 wailian999

JS:   this.name = "x";
来源：http://pcs.hnqzz.top

TS:   name: string = "x";
来源：http://plt.tarul.cn

Java: private String name;
来源：http://heq.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vrv.gaohongyu789.top

Ruby: @name = "x"
来源：http://kxs.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://pzs.gaohongyu789.top

[G04] 定义方法
来源：http://jus.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://faa.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zvh.daxiang520.top

JS:   greet() { return this.name; }
来源：http://wve.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://bpl.wangdashe.top

Java: String greet() { return name; }
来源：http://xzo.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jqu.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://gdz.wangdashe.top

C#:   public string Greet() => Name;
来源：http://yhm.hnxiangtu.top

[G05] 继承
来源：http://gke.havefunace.top

Py:   class Admin(User): pass
来源：http://shh.dianchejie.cn

PHP:  class Admin extends User {}
来源：http://fhl.yj20258.top

JS:   class Admin extends User {}
来源：http://eed.zdbjq.cn

TS:   class Admin extends User {}
来源：http://zuh.mhx1999.top

Java: class Admin extends User {}
来源：http://cqk.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nug.jyoumei.cn

Ruby: class Admin < User; end
来源：http://owl.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://gym.hywenlv.cn

[G06] 重写方法
来源：http://izu.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://hyz.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://igl.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://ono.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://awh.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://zit.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dpz.yongpay.top

Ruby: def greet; "admin"; end
来源：http://bwx.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://vtd.bbcook.cn

[G07] 调用父类方法
来源：http://cdi.tarul.cn

Py:   super().greet()
来源：http://xjg.vehdjk.com

PHP:  parent::greet();
来源：http://lai.yvedp.cn

JS:   super.greet();
来源：http://epu.kuanghao11.cn

TS:   super.greet();
来源：http://aku.feifeiyinyue.top

Java: super.greet();
来源：http://adw.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zpa.shanyushiyangtech.top

Ruby: super
来源：http://mva.sweek.top

C#:   base.Greet();
来源：http://ier.nanxinkj.top

[G08] 静态方法与属性
来源：http://egm.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mjj.yj20258.top

PHP:  public static function f() {}
来源：http://klp.yvedp.cn

JS:   static f() {}
来源：http://zhw.jlsjyb.cn

TS:   static f(): void {}
来源：http://fyn.ivvv.top

Java: static void f() {}
来源：http://tye.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://luw.zhoulong.xyz

Ruby: def self.f; end
来源：http://pcm.ydjk.org.cn

C#:   public static void F() {}
来源：http://kaq.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://zvb.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://vcf.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nys.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hib.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://yfb.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://jhd.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://gor.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yue.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://xpb.zycfv.cn

[G10] 访问控制
来源：http://wwl.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://dgm.zhengqikj.top

PHP:  public / protected / private
来源：http://kle.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://fmh.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://gim.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://tud.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yev.havefunace.top

Ruby: public / protected / private
来源：http://tpm.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://pmq.bbcook.cn

[G11] getter / setter
来源：http://zkk.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://cxw.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://koz.pycfn.com

JS:   get name() { return this._name; }
来源：http://fvl.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://akx.redwolf501.top

Java: public String getName() { return name; }
来源：http://msx.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qdd.haohaochexian.top

Ruby: attr_accessor :name
来源：http://wjz.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://gys.wangdashe.top

[G12] 对象转字符串
来源：http://rta.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://smi.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rni.cucudq.cn

JS:   toString() { return this.name; }
来源：http://orm.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://qra.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://cwg.316326.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://qzj.vehdjk.com

Ruby: def to_s; @name; end
来源：http://pbc.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://nod.pengpengdd.cyou

[G13] 判断对象类型
来源：http://ggr.zycfv.cn

Py:   isinstance(u, User)
来源：http://dar.jinqigufen.top

PHP:  $u instanceof User
来源：http://afk.jqgfzy.top

JS:   u instanceof User
来源：http://oid.pengpengdd.cyou

TS:   u instanceof User
来源：http://pvq.ywan-chungtsiang.top

Java: u instanceof User
来源：http://pam.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vaq.aizwys.cn

Ruby: u.is_a?(User)
来源：http://xay.daria6918.cn

C#:   u is User
来源：http://piw.ydzc1.top

[G14] 数据类 / record
来源：http://uxj.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vcl.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://wce.jiagoushi.top

JS:   // 无内置：普通类或对象字面量
来源：http://gvn.sweek.top

TS:   type User = { name: string; age: number };
来源：http://uzx.xuanzx.com

Java: record User(String name, int age) {}
来源：http://wag.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://gol.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lll.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://syg.yvedp.cn

[G15] 枚举
来源：http://mtr.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nkl.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lvx.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fdp.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://avz.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://cvf.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fnd.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://joz.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gfk.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://qcm.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ssq.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://ucn.xziqi.cn

JS:   Object.entries(obj)
来源：http://ldm.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://zuo.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qlj.svipenyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cji.uphjek.com

Ruby: obj.instance_variables
来源：http://uws.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://hkh.hongshengwenyu.top

================================================================================
来源：http://eyp.bjfxy.top

H. 异常与错误处理
来源：http://qnj.snrcjt.cn

================================================================================
来源：http://obx.pycfn.com

[H01] try / catch 基础
来源：http://nqg.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lyd.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rri.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dxa.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pnc.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lgb.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ytm.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ksv.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zbg.vehdjk.com

[H02] finally / ensure 收尾
来源：http://jap.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://spt.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hfs.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zie.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bxb.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://elx.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vqw.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://puh.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lve.9152youxi.cn

[H03] 主动抛出异常
来源：http://arl.sweek.top

Py:   raise ValueError("错误信息")
来源：http://lnk.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jof.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://awc.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://qhq.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ecx.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fzz.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ynw.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://dod.jqgfzy.top

[H04] 自定义异常类型
来源：http://xqs.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://hec.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://hmu.daria6918.cn

JS:   class MyError extends Error {}
来源：http://pgc.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://zos.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://yii.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://djb.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://moa.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://ccc.shuidangran.top

[H05] 捕获特定类型
来源：http://iig.gzhubu.top

Py:   except ValueError as e:
来源：http://woz.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wsi.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://set.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://mku.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://rxc.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wuc.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://ygq.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zlw.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://vzx.fehbvm.com

Py:   value = d.get("k") or default
来源：http://utp.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xdr.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://ozb.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://pvl.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lhu.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kqv.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://mml.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://aqd.vqdsnc.cn

[H07] 断言
来源：http://xhn.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://ntk.xylfe.cn

PHP:  assert($x > 0);
来源：http://php.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://ljw.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://cnu.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://err.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qfl.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://zyx.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://hnx.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://xmq.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://eue.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gdz.tianlin.xyz

JS:   e.message;  e.stack
来源：http://snw.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hgr.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ida.zhijiandao.cn

Go:   err.Error()
来源：http://ovk.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://ule.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://ymv.nanxuanxn.top

[H09] 带错误码的异常
来源：http://gcf.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bog.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qjw.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ccv.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pye.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rob.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qze.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qfp.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ooo.haohaochexian.top

[H10] 资源自动释放
来源：http://tep.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ses.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oqp.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bek.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wux.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lry.cheryme.top

Go:   defer f.Close()
来源：http://oxh.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://owf.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://god.cqqwz.cn

================================================================================
来源：http://asm.hammf.cn

I. 正则表达式
来源：http://xno.dianchejie.cn

================================================================================
来源：http://nvw.fehbvm.com

[I01] 判断是否匹配
来源：http://rjh.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oly.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://smc.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://lby.uphjek.com

TS:   /\d+/.test(s)
来源：http://bfu.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qil.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cix.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://okq.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mbn.zhoulong.xyz

[I02] 提取所有匹配
来源：http://uuo.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://znr.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zlp.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kwc.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://kid.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gbl.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mcz.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://cne.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zxq.cheryme.top

[I03] 提取捕获分组
来源：http://uwp.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ukc.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hjl.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://utl.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mpp.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fop.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://moc.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ukv.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://udg.yanxiufei.cn

[I04] 正则替换
来源：http://ide.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://zuw.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lgh.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://twe.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://mne.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wrn.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ofx.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://spw.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rdo.hfpthk.cn

[I05] 按正则拆分
来源：http://fva.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bhg.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rcn.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://xgl.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://ipa.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://nda.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mwa.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://gkd.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vsh.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jwg.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lvt.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jum.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nnt.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://usk.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tnb.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://syk.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cgy.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cdl.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://odl.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xqp.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lec.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://opj.hesvh.cn

TS:   /error/gim
来源：http://gje.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lwa.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vdn.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://zcp.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tti.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://czy.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ckl.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ezy.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zsp.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rur.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mbk.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aas.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ftd.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://crr.zhiwuduotai.top

================================================================================
来源：http://cqs.aibaodan.cn

J. 日期与时间
来源：http://xrz.cashguo.top

================================================================================
来源：http://bff.jlsjyb.cn

[J01] 获取当前时间
来源：http://brz.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tfz.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tcc.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://lra.jianghu66.top

TS:   new Date();  Date.now()
来源：http://gjd.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dkg.jiagoushi.top


<!-- 参考信息 -->