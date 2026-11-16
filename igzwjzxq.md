代发 wailian999

[G06] 重写方法
来源：http://jhj.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://dxl.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wqn.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://wje.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://dkf.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://ous.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://grm.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://apm.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://poq.feifeiyinyue.top

[G07] 调用父类方法
来源：http://yga.nwbrower.top

Py:   super().greet()
来源：http://dgy.nwbrower.top

PHP:  parent::greet();
来源：http://enc.zhongyouzk.top

JS:   super.greet();
来源：http://lfg.birdmap.top

TS:   super.greet();
来源：http://mnc.zhengqikj.top

Java: super.greet();
来源：http://qyf.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ihl.gaohongyu789.top

Ruby: super
来源：http://pxl.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://yab.fzhhl.top

[G08] 静态方法与属性
来源：http://peb.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://azm.zhoulong.xyz

PHP:  public static function f() {}
来源：http://rxb.zhixingplan.top

JS:   static f() {}
来源：http://lvm.wangdashe.top

TS:   static f(): void {}
来源：http://mxj.zhixingplan.top

Java: static void f() {}
来源：http://awy.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://uir.jinyuanbaomall.cn

Ruby: def self.f; end
来源：http://xlk.aizwys.cn

C#:   public static void F() {}
来源：http://mja.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://itv.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://qoe.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rqq.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hdi.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://etw.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://ern.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://lzj.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uvc.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://jci.hfpthk.cn

[G10] 访问控制
来源：http://afe.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://gjc.jinqigufen.top

PHP:  public / protected / private
来源：http://xyp.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://fqk.chenjidiqi.icu

TS:   public / protected / private
来源：http://kws.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://xhj.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eni.yj20258.top

Ruby: public / protected / private
来源：http://jxc.gaohongyu789.top

C#:   public / protected / private / internal
来源：http://mbl.birdmap.top

[G11] getter / setter
来源：http://plp.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://bqj.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://iys.guannengcc.top

JS:   get name() { return this._name; }
来源：http://mna.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://xwr.hysaishi.cn

Java: public String getName() { return name; }
来源：http://pfa.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qbm.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://cyt.fktsv.cn

C#:   public string Name { get; set; }
来源：http://xws.zhiwuduotai.top

[G12] 对象转字符串
来源：http://fog.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://efn.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hxp.havefunace.top

JS:   toString() { return this.name; }
来源：http://jca.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://gen.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://rrg.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://tjo.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://wxk.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://yzs.bbcook.cn

[G13] 判断对象类型
来源：http://rnh.zdbjq.cn

Py:   isinstance(u, User)
来源：http://sjd.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://pxt.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://wyx.hnqzz.top

TS:   u instanceof User
来源：http://ceb.jqgfzy.top

Java: u instanceof User
来源：http://fdx.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://udo.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://dyk.aizwys.cn

C#:   u is User
来源：http://upa.hammf.cn

[G14] 数据类 / record
来源：http://bra.zhongyouzk.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ers.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://wmv.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://ltk.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://yhf.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://dmb.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://tjx.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://owh.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://vqf.sjlbkw.cn

[G15] 枚举
来源：http://ixy.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://imt.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lwi.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bnv.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xdm.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://suz.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://axa.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://rmm.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vhe.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://wsd.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hcq.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://zhv.sufxvd.cn

JS:   Object.entries(obj)
来源：http://iky.nwbrower.top

TS:   Object.entries(obj)
来源：http://wqq.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uaq.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tps.jqgufenzy.top

Ruby: obj.instance_variables
来源：http://zhv.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://odp.guannengcc.top

================================================================================
来源：http://mgu.daxiang520.top

H. 异常与错误处理
来源：http://tnz.chenjidiqi.icu

================================================================================
来源：http://qea.yueranfly.top

[H01] try / catch 基础
来源：http://aeg.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fgs.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ybz.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://arm.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://erk.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kdl.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lvf.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gws.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jdy.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://nfk.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://upp.chenjidiqi.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://yxc.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xgg.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uqw.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jew.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lyk.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hqw.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xhq.zhijiandao.cn

[H03] 主动抛出异常
来源：http://rsz.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://jyd.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ddl.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://miu.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://ayg.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vcj.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uaz.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://xei.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://kjd.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://fzo.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://iiv.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://zuj.jianghu66.top

JS:   class MyError extends Error {}
来源：http://qvn.yj20258.top

TS:   class MyError extends Error {}
来源：http://yzj.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://fmo.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ozi.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://rwh.sysykeji.top

C#:   class MyException : Exception {}
来源：http://cea.jlsjyb.cn

[H05] 捕获特定类型
来源：http://pnz.zdqjudy.top

Py:   except ValueError as e:
来源：http://kdu.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lii.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://xjc.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://mfa.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://ngs.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qzi.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://cla.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nun.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://eow.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://zho.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://pfg.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://prv.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://jka.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://req.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yrc.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://jei.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://tlj.yueranfly.top

[H07] 断言
来源：http://koe.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://awu.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://eal.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://izl.redwolf501.top

TS:   console.assert(x > 0);
来源：http://ecq.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://iuk.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nlh.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://aml.zhixingplan.top

C#:   Debug.Assert(x > 0);
来源：http://flq.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://mnh.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://cod.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uxe.jqgfzy.top

JS:   e.message;  e.stack
来源：http://cdf.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://coj.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lzi.jlsjyb.cn

Go:   err.Error()
来源：http://aiu.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://cjg.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://wkd.uphjek.com

[H09] 带错误码的异常
来源：http://riz.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ael.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kpt.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cli.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qzd.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://acu.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cyl.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qwm.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://itt.cucudq.cn

[H10] 资源自动释放
来源：http://cze.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rqk.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://koa.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uni.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qfg.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ivw.yongpay.top

Go:   defer f.Close()
来源：http://hqr.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gch.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eml.pycfn.com

================================================================================
来源：http://kaj.uphjek.com

I. 正则表达式
来源：http://nne.feifeiyinyue.top

================================================================================
来源：http://njr.yanxiufei.cn

[I01] 判断是否匹配
来源：http://blv.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iox.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://ppg.316326.xyz

JS:   /\d+/.test(s)
来源：http://vyy.birdmap.top

TS:   /\d+/.test(s)
来源：http://fgd.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lar.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gky.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://uzk.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jno.chenlongwang.top

[I02] 提取所有匹配
来源：http://tks.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://znm.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wzy.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xsv.yj202588.top

TS:   s.match(/\d+/g)
来源：http://rzv.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://snq.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eij.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://nes.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ybm.iojbl.cn

[I03] 提取捕获分组
来源：http://kau.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://keh.ybcxt.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nyv.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qfn.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://plt.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://itv.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://osp.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zhm.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zun.hcnkem.com

[I04] 正则替换
来源：http://mhy.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://plt.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gpf.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://ikt.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zri.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://jix.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://caj.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zub.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://chn.ppjwa.cn

[I05] 按正则拆分
来源：http://cfq.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wxo.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pym.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://cek.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://gac.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://jzo.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zhk.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dvs.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yjm.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://asy.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dej.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zxf.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ems.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bvd.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ptz.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ryj.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pkl.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://swa.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://ypt.ybcxt.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qbz.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ctz.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ybr.cqqwz.cn

TS:   /error/gim
来源：http://lqs.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bam.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hyf.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://ehh.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qzv.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://yde.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ibh.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nvx.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hvb.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vvf.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kej.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ldg.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jdy.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://thl.daria6918.cn

================================================================================
来源：http://gyt.tian-w.cn

J. 日期与时间
来源：http://dtl.yangfankeji.com

================================================================================
来源：http://skb.quarkkingdee.top

[J01] 获取当前时间
来源：http://vvi.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://muv.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nuf.tanke756.top

JS:   new Date();  Date.now()
来源：http://tpl.uphjek.com

TS:   new Date();  Date.now()
来源：http://bqq.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sqn.hnqzz.top

Go:   time.Now()
来源：http://hoy.hnqzz.top

Ruby: Time.now
来源：http://emm.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wbk.0kj1m.cn

[J02] 格式化输出
来源：http://zuw.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jqc.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://shi.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xtl.hfpthk.cn

TS:   d.toISOString()
来源：http://zqs.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gda.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cna.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqx.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://noz.jianghu66.top

[J03] 字符串解析为日期
来源：http://ojx.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fqm.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fef.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://oge.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://crp.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://nta.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vvi.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://arz.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mwq.xinyue.icu

[J04] 时间戳与日期互转
来源：http://khz.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cvq.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sfl.chenzaomai.com


<!-- 参考信息 -->