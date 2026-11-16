代发 wailian999

Py:   class Admin(User): pass
来源：http://ain.meibo888.top

PHP:  class Admin extends User {}
来源：http://edi.yonumen.top

JS:   class Admin extends User {}
来源：http://xfy.yuanzhike.top

TS:   class Admin extends User {}
来源：http://siq.yonumen.top

Java: class Admin extends User {}
来源：http://ewj.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cjw.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://ewl.hcnkem.com

C#:   class Admin : User {}
来源：http://gnn.mhx1999.top

[G06] 重写方法
来源：http://yfy.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://agv.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yzn.havefunace.top

JS:   greet() { return "admin"; }
来源：http://hez.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://kcl.yueranfly.top

Java: @Override String greet() { return "admin"; }
来源：http://xti.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zqb.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://rcp.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://enx.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://fas.hesvh.cn

Py:   super().greet()
来源：http://atj.yfazqb.com

PHP:  parent::greet();
来源：http://eed.bbcook.cn

JS:   super.greet();
来源：http://xxc.jinqigfzy.top

TS:   super.greet();
来源：http://vwy.gaohongyu789.top

Java: super.greet();
来源：http://vhz.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yet.haohaochexian.top

Ruby: super
来源：http://ngw.0kj1m.cn

C#:   base.Greet();
来源：http://jaf.yj202588.top

[G08] 静态方法与属性
来源：http://jee.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pok.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://ytc.xuetiantiany.cn

JS:   static f() {}
来源：http://wgw.jinqigfzy.top

TS:   static f(): void {}
来源：http://jhv.nanxuanxn.top

Java: static void f() {}
来源：http://eez.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xke.chenzaomai.com

Ruby: def self.f; end
来源：http://tuo.9152youxi.cn

C#:   public static void F() {}
来源：http://yiq.guannengcc.top

[G09] 接口 / 抽象类
来源：http://fzv.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://rvy.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://atc.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://hkq.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://oll.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://bxt.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://hrt.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eql.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://nba.meibo888.top

[G10] 访问控制
来源：http://hxh.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://bcy.yuxming.cn

PHP:  public / protected / private
来源：http://ocx.pycfn.com

JS:   #private 字段；其余公开
来源：http://bbz.zdbjq.cn

TS:   public / protected / private
来源：http://ejx.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://klo.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://job.smart0.xyz

Ruby: public / protected / private
来源：http://yjl.andypj.xyz

C#:   public / protected / private / internal
来源：http://mzs.yj20258888.top

[G11] getter / setter
来源：http://pbs.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://hll.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dli.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://olz.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://eyf.bbcook.cn

Java: public String getName() { return name; }
来源：http://mqp.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zlk.guannengcc.top

Ruby: attr_accessor :name
来源：http://mxe.yfazqb.com

C#:   public string Name { get; set; }
来源：http://lif.vehdjk.com

[G12] 对象转字符串
来源：http://itb.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://bjn.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://off.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://gff.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://vyq.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://xii.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://kyk.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://qha.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://xen.jinqigufen.top

[G13] 判断对象类型
来源：http://rnp.birdmap.top

Py:   isinstance(u, User)
来源：http://dwg.yj20258.top

PHP:  $u instanceof User
来源：http://vdo.aibaodan.cn

JS:   u instanceof User
来源：http://zqm.gotoacloud.top

TS:   u instanceof User
来源：http://yuf.jyoumei.cn

Java: u instanceof User
来源：http://uhj.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hah.cucudq.cn

Ruby: u.is_a?(User)
来源：http://iis.daria6918.cn

C#:   u is User
来源：http://arv.chenzaomai.com

[G14] 数据类 / record
来源：http://ggu.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://out.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://yfb.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://ryf.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://qvf.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://hkp.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://rba.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pzd.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://zht.ybcxt.top

[G15] 枚举
来源：http://mkb.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ndq.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fvj.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bcp.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://isg.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://zqo.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pkf.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://huf.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bsp.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://vcg.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cah.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://xcn.fktsv.cn

JS:   Object.entries(obj)
来源：http://cgy.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://aio.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://afp.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tco.chenzaomai.com

Ruby: obj.instance_variables
来源：http://kci.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://ttf.yangfankeji.com

================================================================================
来源：http://hev.316326.xyz

H. 异常与错误处理
来源：http://aor.wangshuangyany.cn

================================================================================
来源：http://jbz.hcnkem.com

[H01] try / catch 基础
来源：http://ode.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xte.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ahu.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gmu.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lur.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://emt.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hgf.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eub.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wck.yj202588.top

[H02] finally / ensure 收尾
来源：http://dqw.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://tjx.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://rdb.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://arq.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ogn.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://rko.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zbh.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yoc.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ukk.ehwqpu.com

[H03] 主动抛出异常
来源：http://umw.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://ytz.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://elb.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://efp.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://ggn.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zbb.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ybv.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://yzz.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://poi.hnxiangtu.top

[H04] 自定义异常类型
来源：http://grg.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://mmx.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://esi.yongpay.top

JS:   class MyError extends Error {}
来源：http://sok.havefunace.top

TS:   class MyError extends Error {}
来源：http://uzl.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://ebf.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ssr.xingfuxueyuan.xyz

Ruby: class MyError < StandardError; end
来源：http://myz.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://qqw.mhx1999.top

[H05] 捕获特定类型
来源：http://anx.ydjk.org.cn

Py:   except ValueError as e:
来源：http://gst.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xip.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://nix.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://guv.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://ugd.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://atw.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://lbp.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uwk.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://npl.wangdashe.top

Py:   value = d.get("k") or default
来源：http://asm.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://val.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://vxf.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hfy.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://onn.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://aqv.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://ben.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://rbr.shzxlz.cn

[H07] 断言
来源：http://zeq.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://nzq.chenlongwang.top

PHP:  assert($x > 0);
来源：http://izv.tarul.cn

JS:   console.assert(x > 0);
来源：http://zrb.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://wai.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://jaj.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fti.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://njg.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://dgn.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://eqd.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://gbo.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mrr.smart0.xyz

JS:   e.message;  e.stack
来源：http://tur.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gwb.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://czn.epnwcf.com

Go:   err.Error()
来源：http://pul.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://vmi.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://fkm.meibo888.top

[H09] 带错误码的异常
来源：http://cka.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oiq.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://daa.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://prw.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vpl.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://glm.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vxe.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://idt.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kim.chenlongwang.top

[H10] 资源自动释放
来源：http://pni.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://luo.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://roj.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sih.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vlo.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sgf.mhx1999.top

Go:   defer f.Close()
来源：http://wit.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lnh.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ssa.tanke756.top

================================================================================
来源：http://pno.nanxuanxn.top

I. 正则表达式
来源：http://nbd.hnxiangtu.top

================================================================================
来源：http://vql.daxiang520.top

[I01] 判断是否匹配
来源：http://jyx.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bkh.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tqq.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://fnf.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://rwj.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sft.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ovy.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://apr.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bnt.yanxiufei.cn

[I02] 提取所有匹配
来源：http://ilm.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://lqj.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://urw.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lna.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://dms.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mwn.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ntx.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://hzu.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gom.guannengcc.top

[I03] 提取捕获分组
来源：http://mqg.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jgt.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ahx.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wtp.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://muk.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bwr.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iho.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ras.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ypo.ybcxt.top

[I04] 正则替换
来源：http://jsk.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yhj.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://adj.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://kab.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://cse.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cwn.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qou.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nel.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://klr.havefunace.top

[I05] 按正则拆分
来源：http://xvb.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nxe.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vbl.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://sct.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://lfa.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://jsp.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mfk.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://waz.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ydy.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dnw.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hhi.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aoo.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xyd.zhongyouzk.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ubn.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zcb.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dma.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zxl.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wik.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://cml.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://stw.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sqo.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lzz.fzhhl.top

TS:   /error/gim
来源：http://gwj.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wpu.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qhd.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://sqk.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cle.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://gpr.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oxp.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hlg.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sul.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://psj.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mkf.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ufv.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ubi.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dfs.yongpay.top

================================================================================
来源：http://nij.wangdashe.top

J. 日期与时间
来源：http://uwu.zhengqikj.top

================================================================================
来源：http://kbw.nanxinkj.top

[J01] 获取当前时间
来源：http://okj.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://oep.xuanzx.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mav.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://awt.hcnkem.com

TS:   new Date();  Date.now()
来源：http://udl.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://xeu.wangdashe.top

Go:   time.Now()
来源：http://fve.zdqjudy.top

Ruby: Time.now
来源：http://jqx.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ods.guowangkeji.top

[J02] 格式化输出
来源：http://ztn.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://khy.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tqw.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aiy.yongpay.top

TS:   d.toISOString()
来源：http://brr.mhx1999.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://voy.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://luk.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yja.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://prx.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://vxx.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://suq.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xqv.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://usp.daria6918.cn


<!-- 参考信息 -->