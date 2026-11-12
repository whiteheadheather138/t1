代发 wailian999

Java: class Admin extends User {}
来源：http://mgq.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nii.tianlin.xyz

Ruby: class Admin < User; end
来源：http://mfo.zdqjudy.top

C#:   class Admin : User {}
来源：http://ipf.meibo888.top

[G06] 重写方法
来源：http://xvm.birdmap.top

Py:   def greet(self): return "admin"
来源：http://mnm.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ycn.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://wbp.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://zsq.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://fub.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sae.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://ahu.sweek.top

C#:   public override string Greet() => "admin";
来源：http://pxn.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://qcc.jqgufenzy.top

Py:   super().greet()
来源：http://hiy.tian-w.cn

PHP:  parent::greet();
来源：http://nuk.52xcode.cn

JS:   super.greet();
来源：http://erb.bjfxy.top

TS:   super.greet();
来源：http://nhg.guannengcc.top

Java: super.greet();
来源：http://msp.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wit.xuanzx.com

Ruby: super
来源：http://lbx.jqgfzy.top

C#:   base.Greet();
来源：http://bcz.uphjek.com

[G08] 静态方法与属性
来源：http://hih.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oyg.yuanzhike.top

PHP:  public static function f() {}
来源：http://fvs.zycfv.cn

JS:   static f() {}
来源：http://dkz.yfazqb.com

TS:   static f(): void {}
来源：http://lwz.dianchejie.cn

Java: static void f() {}
来源：http://hly.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fzq.tianlin.xyz

Ruby: def self.f; end
来源：http://zqr.shangyingyoupin.top

C#:   public static void F() {}
来源：http://wgx.yvedp.cn

[G09] 接口 / 抽象类
来源：http://kyj.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gze.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rta.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ulj.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://bwc.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://kij.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://exp.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wxs.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://ifw.wangdashe.top

[G10] 访问控制
来源：http://wii.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://vmg.0kj1m.cn

PHP:  public / protected / private
来源：http://cpj.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://xph.hammf.cn

TS:   public / protected / private
来源：http://ewu.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://rdb.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lzg.yongpay.top

Ruby: public / protected / private
来源：http://uic.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://czs.fehbvm.com

[G11] getter / setter
来源：http://yki.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://nuo.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nql.hammf.cn

JS:   get name() { return this._name; }
来源：http://pji.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://ech.guowangkeji.top

Java: public String getName() { return name; }
来源：http://whv.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://euv.jqgfzy.top

Ruby: attr_accessor :name
来源：http://cqu.yongpay.top

C#:   public string Name { get; set; }
来源：http://utb.gotoacloud.top

[G12] 对象转字符串
来源：http://pff.hammf.cn

Py:   def __str__(self): return self.name
来源：http://ous.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ggy.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://cxm.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://skn.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://ibz.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://jqf.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://lqb.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://rqv.yuxming.cn

[G13] 判断对象类型
来源：http://fzw.yuanzhike.top

Py:   isinstance(u, User)
来源：http://xoc.316326.xyz

PHP:  $u instanceof User
来源：http://vge.yj20258888.top

JS:   u instanceof User
来源：http://upe.jlsjyb.cn

TS:   u instanceof User
来源：http://iwa.quarkkingdee.top

Java: u instanceof User
来源：http://awi.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cyd.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://mqv.epnwcf.com

C#:   u is User
来源：http://hou.nwbrower.top

[G14] 数据类 / record
来源：http://dwr.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kse.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://jqx.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://pml.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://zty.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://txi.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://ttj.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ogx.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://aqc.52xcode.cn

[G15] 枚举
来源：http://cxt.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rvd.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vjb.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hjv.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://keg.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://uux.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://efs.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://eiv.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bcw.yj20258.top

[G16] 对象转数组 / 字典
来源：http://ecb.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nbw.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://pjw.zycfv.cn

JS:   Object.entries(obj)
来源：http://jns.xylfe.cn

TS:   Object.entries(obj)
来源：http://hcd.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vqj.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pho.epnwcf.com

Ruby: obj.instance_variables
来源：http://khm.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://ufp.zhijiandao.cn

================================================================================
来源：http://gkh.hammf.cn

H. 异常与错误处理
来源：http://hky.sweek.top

================================================================================
来源：http://dgb.hnxiangtu.top

[H01] try / catch 基础
来源：http://kmk.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yay.aizwys.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gyl.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ugx.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qbh.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dwn.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zsy.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://diu.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://whd.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://kdj.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://gux.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://rza.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xso.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uxy.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://voz.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://fbh.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mug.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yty.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://xod.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://nlo.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ztl.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://zug.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://svy.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mpo.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://khx.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rgh.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ttj.guowangkeji.top

[H04] 自定义异常类型
来源：http://prw.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://rdb.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://boj.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://lyr.havefunace.top

TS:   class MyError extends Error {}
来源：http://qub.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://jdf.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aqu.cqqwz.cn

Ruby: class MyError < StandardError; end
来源：http://mke.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://vuj.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://qho.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://pgt.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://acu.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://fst.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://muj.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://ist.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://phc.yuxming.cn

Ruby: rescue ArgumentError => e
来源：http://mqm.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rwi.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://nkq.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://xkd.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lbl.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rnb.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://yer.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tfr.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fus.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://oll.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://lnk.shanyushiyangtech.top

[H07] 断言
来源：http://gwn.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://yvt.cqqwz.cn

PHP:  assert($x > 0);
来源：http://xhb.cucudq.cn

JS:   console.assert(x > 0);
来源：http://cpg.xuanzx.com

TS:   console.assert(x > 0);
来源：http://wkg.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://dpt.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hha.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://mkv.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://dwg.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://nhl.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://dbl.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kmf.cheryme.top

JS:   e.message;  e.stack
来源：http://pgj.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qoi.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eqx.daria6918.cn

Go:   err.Error()
来源：http://lny.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://tbc.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://bgm.zdqjudy.top

[H09] 带错误码的异常
来源：http://mok.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vbk.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://igw.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hnj.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lxx.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gcn.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://agu.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://gxs.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xdg.wangdashe.top

[H10] 资源自动释放
来源：http://iwk.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://ome.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hol.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yrt.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dsp.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ulg.yvedp.cn

Go:   defer f.Close()
来源：http://rkp.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tdg.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gkm.fengsongda.top

================================================================================
来源：http://xgu.andypj.xyz

I. 正则表达式
来源：http://cmx.zhengqikj.top

================================================================================
来源：http://cbr.zycfv.cn

[I01] 判断是否匹配
来源：http://hwa.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vdk.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pca.nwbrower.top

JS:   /\d+/.test(s)
来源：http://qin.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://oaq.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://efq.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lbh.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://zmv.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dgy.zhoulong.xyz

[I02] 提取所有匹配
来源：http://uly.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://mbi.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://irc.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cqq.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://qit.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wly.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xan.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://bnj.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://izs.iojbl.cn

[I03] 提取捕获分组
来源：http://qyw.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ili.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dxh.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kik.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ptq.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fvx.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mzq.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://faj.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://apb.dashuyun.cn

[I04] 正则替换
来源：http://eql.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yoi.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yja.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://wgc.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://iak.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xhv.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cfo.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://spx.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gbm.ydjk.org.cn

[I05] 按正则拆分
来源：http://gqw.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://gci.hcnkem.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pni.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://zpu.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://qqb.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://dfu.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://npv.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qnl.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yta.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zyn.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xnz.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ipc.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rpx.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tkm.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mis.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gbv.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kdz.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yoh.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://kkb.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qzr.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rnu.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://scq.yj20258888.top

TS:   /error/gim
来源：http://enj.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pxc.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cok.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://qqo.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ojk.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://vbo.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mpn.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rnv.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ocn.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mso.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://twn.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tzh.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bow.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wgn.yongpay.top

================================================================================
来源：http://lcg.svipenyu.cn

J. 日期与时间
来源：http://ntr.ivvv.top

================================================================================
来源：http://cno.quarkkingdee.top

[J01] 获取当前时间
来源：http://yed.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://txa.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nix.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://nti.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://acp.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://wcu.0kj1m.cn

Go:   time.Now()
来源：http://pym.cucudq.cn

Ruby: Time.now
来源：http://mtt.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uag.sjlbkw.cn

[J02] 格式化输出
来源：http://bto.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wcp.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aei.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ecb.sysykeji.top

TS:   d.toISOString()
来源：http://isy.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kbz.jyoumei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jrf.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dvo.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tbl.svipenyu.cn

[J03] 字符串解析为日期
来源：http://ayc.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uvj.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iki.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://vql.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://eve.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://ljw.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cud.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://lbq.shuidangran.top


<!-- 参考信息 -->