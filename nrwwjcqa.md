代发 wailian999

[G06] 重写方法
来源：http://jam.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://jvo.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gdx.yj20258.top

JS:   greet() { return "admin"; }
来源：http://jxn.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://lwt.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://jur.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xuj.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://snz.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://fpy.yvedp.cn

[G07] 调用父类方法
来源：http://xke.c1oappe.top

Py:   super().greet()
来源：http://vvp.xuetiantiany.cn

PHP:  parent::greet();
来源：http://vwd.guannengcc.top

JS:   super.greet();
来源：http://mei.tanke756.top

TS:   super.greet();
来源：http://uel.jianghu66.top

Java: super.greet();
来源：http://xky.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ott.guowangkeji.top

Ruby: super
来源：http://zlj.kuanghao11.cn

C#:   base.Greet();
来源：http://rxi.ydzc1.top

[G08] 静态方法与属性
来源：http://tui.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://egb.tian-w.cn

PHP:  public static function f() {}
来源：http://hkr.shuidangran.top

JS:   static f() {}
来源：http://jdz.pengpengdd.cyou

TS:   static f(): void {}
来源：http://jhf.zhijiandao.cn

Java: static void f() {}
来源：http://zok.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://fvs.shuidangran.top

Ruby: def self.f; end
来源：http://cpn.fzhhl.top

C#:   public static void F() {}
来源：http://pzu.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://xnb.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://gxp.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://tce.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://gqc.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://ram.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://dcj.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://efk.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cjr.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://hhk.wangdashe.top

[G10] 访问控制
来源：http://wfw.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://uxr.redwolf501.top

PHP:  public / protected / private
来源：http://rdu.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://kgx.hesvh.cn

TS:   public / protected / private
来源：http://pjp.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://hhc.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://srd.gaohongyu789.top

Ruby: public / protected / private
来源：http://ely.xinyue.icu

C#:   public / protected / private / internal
来源：http://ivr.ehwqpu.com

[G11] getter / setter
来源：http://jkz.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://cae.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kru.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://wlc.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://jss.gzhubu.top

Java: public String getName() { return name; }
来源：http://kbl.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://krj.xinyue.icu

Ruby: attr_accessor :name
来源：http://idn.iojbl.cn

C#:   public string Name { get; set; }
来源：http://xio.wangshuangyany.cn

[G12] 对象转字符串
来源：http://cyj.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://wpl.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fjm.pycfn.com

JS:   toString() { return this.name; }
来源：http://jfa.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://esx.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://ytk.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://cli.xziqi.cn

Ruby: def to_s; @name; end
来源：http://lry.yj202588.top

C#:   public override string ToString() => Name;
来源：http://tbt.cashguo.top

[G13] 判断对象类型
来源：http://tlp.xylfe.cn

Py:   isinstance(u, User)
来源：http://rml.tanke756.top

PHP:  $u instanceof User
来源：http://svt.uphjek.com

JS:   u instanceof User
来源：http://wyp.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://smf.ybcxt.top

Java: u instanceof User
来源：http://wao.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldy.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://tdt.vehdjk.com

C#:   u is User
来源：http://bfa.gzhubu.top

[G14] 数据类 / record
来源：http://mad.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cve.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://lfj.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://rav.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://agl.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://ncx.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://uud.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dto.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://yks.vehdjk.com

[G15] 枚举
来源：http://tey.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sfx.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hys.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ozt.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jgo.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://ivz.zhengqikj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zuo.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://pwj.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ayl.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://szx.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eun.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://ppz.zycfv.cn

JS:   Object.entries(obj)
来源：http://pvd.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://pfc.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gkz.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://uox.c1oappe.top

Ruby: obj.instance_variables
来源：http://qtp.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://vhe.fzhhl.top

================================================================================
来源：http://yfi.jinqigfzy.top

H. 异常与错误处理
来源：http://aqn.sxryk.cn

================================================================================
来源：http://pzn.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://hgg.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iod.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wvj.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zzz.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://exx.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bgp.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pfp.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://skq.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jui.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://fzx.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://bzh.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vot.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://odj.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://qjd.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eja.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ott.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hzx.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rdo.redwolf501.top

[H03] 主动抛出异常
来源：http://hsb.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://fci.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ngg.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://ihz.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://tnk.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gnf.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ncf.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uzg.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gxr.guowangkeji.top

[H04] 自定义异常类型
来源：http://iqs.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://xsp.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://jkx.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://uvp.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://qgh.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://fpz.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uwk.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://hlh.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://kmg.zhengqikj.top

[H05] 捕获特定类型
来源：http://epx.dianchejie.cn

Py:   except ValueError as e:
来源：http://dgs.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qyc.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://ylb.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://iky.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://uqf.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lkf.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://rfx.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vik.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://jwi.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://fyv.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qbw.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://mis.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://rce.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://klz.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yok.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://blx.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://yzl.jinghuilouyu.cn

[H07] 断言
来源：http://cly.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://cnp.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://ffv.yueranfly.top

JS:   console.assert(x > 0);
来源：http://mip.vehdjk.com

TS:   console.assert(x > 0);
来源：http://vur.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://eyp.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ulg.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kei.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://amx.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://xhn.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://fdj.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nsp.dashuyun.cn

JS:   e.message;  e.stack
来源：http://rkb.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://smv.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uyo.jinqigufen.top

Go:   err.Error()
来源：http://qkc.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://lcm.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://vkb.hesvh.cn

[H09] 带错误码的异常
来源：http://gpv.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zui.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lsx.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ywi.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ysz.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qqv.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yeb.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://dma.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xfd.gaohongyu789.top

[H10] 资源自动释放
来源：http://nfx.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xnc.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://guu.ivvv.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hnd.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jun.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://obl.shuidangran.top

Go:   defer f.Close()
来源：http://wmu.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gaz.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xmg.yvedp.cn

================================================================================
来源：http://amy.tarul.cn

I. 正则表达式
来源：http://wjv.mhx1999.top

================================================================================
来源：http://wqx.zhijiandao.cn

[I01] 判断是否匹配
来源：http://onc.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ixn.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://xdc.iojbl.cn

JS:   /\d+/.test(s)
来源：http://ulk.yj20258.top

TS:   /\d+/.test(s)
来源：http://hyd.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ycc.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lde.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://fsd.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vsb.ppjwa.cn

[I02] 提取所有匹配
来源：http://eip.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://npd.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gyt.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://asm.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://ggp.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://goi.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zpp.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://nxf.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pfd.316326.xyz

[I03] 提取捕获分组
来源：http://bng.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pxw.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ksv.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wam.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vtr.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nfs.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xva.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://olf.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wgv.sxryk.cn

[I04] 正则替换
来源：http://div.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://reo.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ysk.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://agc.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://mih.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://yil.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ldk.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://imh.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nkf.jqgfzy.top

[I05] 按正则拆分
来源：http://jpf.zdqjudy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qdb.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wwz.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://nir.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://nae.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://gpx.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cjg.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://lvl.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eef.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gks.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gvv.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zvy.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wic.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://htj.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mma.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lqh.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rxm.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xjb.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://ypo.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hru.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ufy.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qkq.redwolf501.top

TS:   /error/gim
来源：http://fvi.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://edz.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ldy.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://gem.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rcg.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://qdt.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dki.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tao.zhaomingkeji.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ulf.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fud.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gbj.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://htl.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dri.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kuh.c1oappe.top

================================================================================
来源：http://ilg.yj20258888.top

J. 日期与时间
来源：http://ooo.meibo888.top

================================================================================
来源：http://yzm.guannengcc.top

[J01] 获取当前时间
来源：http://xhe.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kwm.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uai.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://gml.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://fri.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sle.xinyue.icu

Go:   time.Now()
来源：http://ceu.yongpay.top

Ruby: Time.now
来源：http://cck.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fsu.sufxvd.cn

[J02] 格式化输出
来源：http://uhl.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzu.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ora.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rba.zhengqikj.top

TS:   d.toISOString()
来源：http://bkx.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gzx.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qls.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zsb.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lbg.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://ilc.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://abq.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fgq.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://lxo.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://gpc.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uvw.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yvp.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://btr.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxc.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://all.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wpm.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ynb.ppjwa.cn


<!-- 参考信息 -->