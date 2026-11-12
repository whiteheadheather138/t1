代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://pds.cucudq.cn

[G07] 调用父类方法
来源：http://rig.haohaochexian.top

Py:   super().greet()
来源：http://kql.meibo888.top

PHP:  parent::greet();
来源：http://kzj.fehbvm.com

JS:   super.greet();
来源：http://ufo.yj202588.top

TS:   super.greet();
来源：http://prj.zhixingplan.top

Java: super.greet();
来源：http://dal.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rqp.yuxming.cn

Ruby: super
来源：http://iga.chenjidiqi.icu

C#:   base.Greet();
来源：http://vmx.wangshuangyany.cn

[G08] 静态方法与属性
来源：http://ica.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ngl.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://vst.ctjpmb.com

JS:   static f() {}
来源：http://jqm.52xcode.cn

TS:   static f(): void {}
来源：http://thb.yongpay.top

Java: static void f() {}
来源：http://pez.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dth.ivvv.top

Ruby: def self.f; end
来源：http://pha.hongshengwenyu.top

C#:   public static void F() {}
来源：http://gyf.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://pef.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://rnt.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://rqc.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uxi.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://rzq.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://xyn.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://hvz.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cwi.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://jaf.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://phe.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://wyg.tarul.cn

PHP:  public / protected / private
来源：http://rxg.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://vdt.aizwys.cn

TS:   public / protected / private
来源：http://ate.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://xts.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://vdi.xylfe.cn

Ruby: public / protected / private
来源：http://mvl.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://pym.wangshuangyany.cn

[G11] getter / setter
来源：http://yvz.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://ogj.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://che.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://odx.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://vze.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://gse.jyoumei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kaz.xuanzx.com

Ruby: attr_accessor :name
来源：http://zjf.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://emq.yuxming.cn

[G12] 对象转字符串
来源：http://hsz.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://xqw.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ouh.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://bst.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://yex.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://how.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ivy.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://ode.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://puk.meibo888.top

[G13] 判断对象类型
来源：http://uxi.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://fjq.9152youxi.cn

PHP:  $u instanceof User
来源：http://ezx.0kj1m.cn

JS:   u instanceof User
来源：http://ust.ydzc1.top

TS:   u instanceof User
来源：http://vil.yongpay.top

Java: u instanceof User
来源：http://ekj.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mza.yj20258.top

Ruby: u.is_a?(User)
来源：http://fmy.dashuyun.cn

C#:   u is User
来源：http://rzp.sjlbkw.cn

[G14] 数据类 / record
来源：http://ylq.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wuj.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://ele.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://pyc.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://rdg.sweek.top

Java: record User(String name, int age) {}
来源：http://opl.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://nde.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://phi.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://dnu.pengpengdd.cyou

[G15] 枚举
来源：http://ejz.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rmb.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://crn.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://euq.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fcr.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://xst.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oye.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://xbv.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ohd.hammf.cn

[G16] 对象转数组 / 字典
来源：http://mfn.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sud.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://lri.andypj.xyz

JS:   Object.entries(obj)
来源：http://yfv.sweek.top

TS:   Object.entries(obj)
来源：http://uxv.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hja.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pbh.mhx1999.top

Ruby: obj.instance_variables
来源：http://imw.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://uhw.fzhhl.top

================================================================================
来源：http://kpx.feifeiyinyue.top

H. 异常与错误处理
来源：http://auv.epnwcf.com

================================================================================
来源：http://zcq.zhiwuduotai.top

[H01] try / catch 基础
来源：http://lip.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ldg.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fvi.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qam.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baz.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fxb.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://otm.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ohn.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://evb.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://mzx.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://vib.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fon.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lbi.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dme.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://alt.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nua.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qdx.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pmh.jinqigfzy.top

[H03] 主动抛出异常
来源：http://qrp.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://lyx.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wwr.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://mzr.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://iwh.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dmj.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zjr.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ujy.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://ifk.sufxvd.cn

[H04] 自定义异常类型
来源：http://yfb.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://ygp.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pqz.hnqzz.top

JS:   class MyError extends Error {}
来源：http://fxt.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://adz.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://nes.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mwo.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://umt.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://drh.ydzc1.top

[H05] 捕获特定类型
来源：http://ktw.zhoulong.xyz

Py:   except ValueError as e:
来源：http://jcr.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zwz.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://fre.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://gtc.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://qjr.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nji.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://rvq.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cyf.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://zjs.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://rkv.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://nnr.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://jns.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rfe.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rnx.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://quh.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://ysc.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://sew.shuidangran.top

[H07] 断言
来源：http://ujb.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://epl.hnqzz.top

PHP:  assert($x > 0);
来源：http://qji.wangdashe.top

JS:   console.assert(x > 0);
来源：http://zio.uphjek.com

TS:   console.assert(x > 0);
来源：http://doq.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://mak.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pyp.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://oup.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://lrb.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://jpd.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://ovh.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nqj.snrcjt.cn

JS:   e.message;  e.stack
来源：http://its.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lit.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ozr.dianchejie.cn

Go:   err.Error()
来源：http://tdg.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://lms.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://fcc.yongpay.top

[H09] 带错误码的异常
来源：http://hie.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://inv.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xps.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xhq.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yuq.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kzn.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bjq.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://uwn.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rul.aibaodan.cn

[H10] 资源自动释放
来源：http://ogv.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uya.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gki.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wzi.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ctg.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kyy.jinqigfzy.top

Go:   defer f.Close()
来源：http://eva.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cht.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sgu.yonumen.top

================================================================================
来源：http://vlm.haohaochexian.top

I. 正则表达式
来源：http://fwy.ctjpmb.com

================================================================================
来源：http://gmc.jqgfzy.top

[I01] 判断是否匹配
来源：http://amk.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://krr.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://ubc.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://oqe.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://pmo.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uau.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://owo.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://agr.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vne.aizwys.cn

[I02] 提取所有匹配
来源：http://ecr.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://dnh.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qpn.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gfa.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://mzw.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wby.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vch.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://uzf.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qdc.yvedp.cn

[I03] 提取捕获分组
来源：http://imb.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ggc.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tph.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cuq.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://que.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://krv.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://erp.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bfb.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sea.wangdashe.top

[I04] 正则替换
来源：http://pva.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ycb.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mps.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://tde.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://uvv.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://nux.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vzo.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zth.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gwv.ivvv.top

[I05] 按正则拆分
来源：http://bqx.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://wiu.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ltj.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://ymo.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://sqh.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://jow.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pay.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ngv.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vul.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://njx.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ysw.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mnd.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ofl.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bin.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://byf.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jsc.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jys.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://urc.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://mge.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://npc.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fwp.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qor.c1oappe.top

TS:   /error/gim
来源：http://dlh.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wcd.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ich.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://gof.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dyj.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://cty.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kgs.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cji.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aps.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qwi.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wcd.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ybl.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vxn.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ozn.jiagoushi.top

================================================================================
来源：http://tdj.xingfuxueyuan.xyz

J. 日期与时间
来源：http://dvb.chenzaomai.com

================================================================================
来源：http://vmh.zhongyouzk.top

[J01] 获取当前时间
来源：http://ycm.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oil.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dtf.yuxming.cn

JS:   new Date();  Date.now()
来源：http://paf.bbcook.cn

TS:   new Date();  Date.now()
来源：http://dhh.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kfq.nwbrower.top

Go:   time.Now()
来源：http://ant.havefunace.top

Ruby: Time.now
来源：http://iqe.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://udt.hongshengwenyu.top

[J02] 格式化输出
来源：http://rjp.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lrf.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hsh.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sas.hywenlv.cn

TS:   d.toISOString()
来源：http://tmf.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xow.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qdr.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uiu.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hkk.hcnkem.com

[J03] 字符串解析为日期
来源：http://ylv.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jwm.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xki.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://obn.hammf.cn

TS:   new Date("2024-01-02")
来源：http://gpm.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yrg.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://klb.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://zwn.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gre.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://ekf.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rbv.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qzi.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pec.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xej.mhx1999.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gfm.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sem.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbu.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iue.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://rtr.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ejo.yj20258888.top


<!-- 参考信息 -->