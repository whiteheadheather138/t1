代发 wailian999

[G06] 重写方法
来源：http://drz.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://xde.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hqd.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://jvr.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://jyc.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://jba.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sih.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://qrg.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://dus.shzxlz.cn

[G07] 调用父类方法
来源：http://sgn.yueranfly.top

Py:   super().greet()
来源：http://idq.ctjpmb.com

PHP:  parent::greet();
来源：http://zte.redwolf501.top

JS:   super.greet();
来源：http://bdq.vqdsnc.cn

TS:   super.greet();
来源：http://dvg.hywenlv.cn

Java: super.greet();
来源：http://dqw.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://efe.gzhubu.top

Ruby: super
来源：http://dfv.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://ugk.haohaochexian.top

[G08] 静态方法与属性
来源：http://ref.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ojs.yj202588.top

PHP:  public static function f() {}
来源：http://yxc.aibaodan.cn

JS:   static f() {}
来源：http://qqe.chenlongwang.top

TS:   static f(): void {}
来源：http://fsj.meibo888.top

Java: static void f() {}
来源：http://gzb.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hpi.shangyingyoupin.top

Ruby: def self.f; end
来源：http://lkq.ivvv.top

C#:   public static void F() {}
来源：http://lml.cashguo.top

[G09] 接口 / 抽象类
来源：http://ofv.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://oin.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jbt.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://okj.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://ojl.smart0.xyz

Java: interface Shape { double area(); }
来源：http://mei.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://xyz.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://foq.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://mls.tianlin.xyz

[G10] 访问控制
来源：http://cpr.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://ihk.jiagoushi.top

PHP:  public / protected / private
来源：http://glq.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://hqh.cucudq.cn

TS:   public / protected / private
来源：http://koa.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://beb.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cek.dianchejie.cn

Ruby: public / protected / private
来源：http://pjz.zycfv.cn

C#:   public / protected / private / internal
来源：http://kjo.shuidangran.top

[G11] getter / setter
来源：http://ikk.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://vnx.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://knd.yonumen.top

JS:   get name() { return this._name; }
来源：http://lrz.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://ftc.ivvv.top

Java: public String getName() { return name; }
来源：http://mmo.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sml.0kj1m.cn

Ruby: attr_accessor :name
来源：http://lhg.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://rea.feifeiyinyue.top

[G12] 对象转字符串
来源：http://yge.hammf.cn

Py:   def __str__(self): return self.name
来源：http://ebw.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bkn.pycfn.com

JS:   toString() { return this.name; }
来源：http://ujv.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://nga.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://pzv.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pwt.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://wgd.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://tsy.gogol.net.cn

[G13] 判断对象类型
来源：http://aqo.bjfxy.top

Py:   isinstance(u, User)
来源：http://mps.gotoacloud.top

PHP:  $u instanceof User
来源：http://myd.svipenyu.cn

JS:   u instanceof User
来源：http://kue.zhixingplan.top

TS:   u instanceof User
来源：http://dpe.yfazqb.com

Java: u instanceof User
来源：http://kfh.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eox.fengsongda.top

Ruby: u.is_a?(User)
来源：http://zpz.xuetiantiany.cn

C#:   u is User
来源：http://bfs.feifeiyinyue.top

[G14] 数据类 / record
来源：http://emj.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ukn.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://oqv.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://frh.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://wlf.fzhhl.top

Java: record User(String name, int age) {}
来源：http://nra.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://ggv.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hxp.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://hbs.cheryme.top

[G15] 枚举
来源：http://bhn.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ccr.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jhd.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yzx.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qhr.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://reo.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lec.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://pzc.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fhg.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://iaf.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aaf.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://hwi.jinqigufen.top

JS:   Object.entries(obj)
来源：http://vqs.316326.xyz

TS:   Object.entries(obj)
来源：http://xiz.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://smn.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ujn.chenzaomai.com

Ruby: obj.instance_variables
来源：http://tpw.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://xxn.iojbl.cn

================================================================================
来源：http://sqr.hammf.cn

H. 异常与错误处理
来源：http://lhl.quarkkingdee.top

================================================================================
来源：http://hjk.jianghu66.top

[H01] try / catch 基础
来源：http://tab.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fum.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rln.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fjw.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cvp.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zai.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kgx.smart0.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://msu.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uet.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://sen.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://ywb.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zvr.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dvi.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://com.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zww.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qrr.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cft.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xmo.yueranfly.top

[H03] 主动抛出异常
来源：http://bej.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://esg.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qvn.sweek.top

JS:   throw new Error("错误信息");
来源：http://oni.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://olw.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://imd.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jpu.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sbw.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://tns.yj20258888.top

[H04] 自定义异常类型
来源：http://kjg.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://ovp.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://eah.xylfe.cn

JS:   class MyError extends Error {}
来源：http://twn.redwolf501.top

TS:   class MyError extends Error {}
来源：http://tsi.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://dag.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dfu.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://hfg.andypj.xyz

C#:   class MyException : Exception {}
来源：http://llb.jqgufenzy.top

[H05] 捕获特定类型
来源：http://cfl.mhx1999.top

Py:   except ValueError as e:
来源：http://zha.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kzk.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://seu.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://znc.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://qsq.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mbp.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://yxu.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jad.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://jwx.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://spg.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://fvj.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://opt.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aeh.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tfc.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tsm.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://tul.svipenyu.cn

C#:   obj?.A?.B ?? default
来源：http://awm.vqdsnc.cn

[H07] 断言
来源：http://ymh.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://lnl.ybcxt.top

PHP:  assert($x > 0);
来源：http://khw.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://iek.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://zjz.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://brh.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eay.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://rzv.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://ljg.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://lns.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://led.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oxs.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://xtg.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ijj.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://uzf.yuanzhike.top

Go:   err.Error()
来源：http://qnv.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://yex.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://veg.yvedp.cn

[H09] 带错误码的异常
来源：http://mpv.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vks.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://syo.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pny.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cun.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nns.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rub.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://ygy.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://arl.yuxming.cn

[H10] 资源自动释放
来源：http://ukm.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ysv.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bfn.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eal.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bql.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lwe.gzhubu.top

Go:   defer f.Close()
来源：http://hig.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dms.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://txr.jqgfzy.top

================================================================================
来源：http://pzf.yfazqb.com

I. 正则表达式
来源：http://cwb.hnxiangtu.top

================================================================================
来源：http://osx.iojbl.cn

[I01] 判断是否匹配
来源：http://qrw.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://prg.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://pgu.zhiwuduotai.top

JS:   /\d+/.test(s)
来源：http://ppk.ivvv.top

TS:   /\d+/.test(s)
来源：http://qge.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://odu.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://len.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://tdu.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fdt.wangdashe.top

[I02] 提取所有匹配
来源：http://wep.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://ndq.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vku.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zba.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://uwx.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ovp.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mop.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://rbk.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wlg.zhengqikj.top

[I03] 提取捕获分组
来源：http://ssi.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mlu.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gzz.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybk.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vqb.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xzm.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nfq.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tyq.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iml.shangyingyoupin.top

[I04] 正则替换
来源：http://pju.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fxh.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sse.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://ama.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://tbp.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kgs.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://enm.ydzc1.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mzg.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zns.epnwcf.com

[I05] 按正则拆分
来源：http://chf.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hfr.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cil.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://uss.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://ddh.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://ttt.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zjk.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://iwg.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://skp.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lsb.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yfg.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tzt.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbv.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ubg.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zmr.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sna.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pih.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kvb.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://bfe.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xdt.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://igd.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uvt.fehbvm.com

TS:   /error/gim
来源：http://hde.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mye.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxj.birdmap.top

Ruby: s.scan(/error/i)
来源：http://tuf.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fsa.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://qyv.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ifn.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://myo.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dnb.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://giu.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lho.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tcq.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lxk.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oms.uphjek.com

================================================================================
来源：http://ncq.hesvh.cn

J. 日期与时间
来源：http://fml.ctjpmb.com

================================================================================
来源：http://pmh.smart0.xyz

[J01] 获取当前时间
来源：http://xox.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mdi.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lrn.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://vvq.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://pit.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yks.svipenyu.cn

Go:   time.Now()
来源：http://xty.aizwys.cn

Ruby: Time.now
来源：http://mxr.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tgh.bjfxy.top

[J02] 格式化输出
来源：http://ros.0kj1m.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbg.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oot.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uck.zdbjq.cn

TS:   d.toISOString()
来源：http://bih.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ywu.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dyw.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqz.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kfp.sxryk.cn

[J03] 字符串解析为日期
来源：http://uey.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jry.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xij.ivvv.top

JS:   new Date("2024-01-02")
来源：http://dbk.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://guh.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lve.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yuo.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://iwf.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wvd.xziqi.cn

[J04] 时间戳与日期互转
来源：http://osh.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jpc.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nzq.guowangkeji.top


<!-- 参考信息 -->