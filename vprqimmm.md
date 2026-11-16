代发 wailian999

Py:   class Admin(User): pass
来源：http://ypw.fengsongda.top

PHP:  class Admin extends User {}
来源：http://umz.yuxming.cn

JS:   class Admin extends User {}
来源：http://pur.xinyue.icu

TS:   class Admin extends User {}
来源：http://fqy.fktsv.cn

Java: class Admin extends User {}
来源：http://lou.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://beg.sxryk.cn

Ruby: class Admin < User; end
来源：http://uzy.shzxlz.cn

C#:   class Admin : User {}
来源：http://hrd.shanyushiyangkeji.top

[G06] 重写方法
来源：http://jen.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://cdg.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wbq.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://nzs.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://tul.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://pvb.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uhx.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://ttm.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://jyt.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://hyf.jinqigfzy.top

Py:   super().greet()
来源：http://wkf.hammf.cn

PHP:  parent::greet();
来源：http://xrl.vehdjk.com

JS:   super.greet();
来源：http://ehc.daxiang520.top

TS:   super.greet();
来源：http://pht.cheryme.top

Java: super.greet();
来源：http://mot.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://riw.gotoacloud.top

Ruby: super
来源：http://jgs.hfpthk.cn

C#:   base.Greet();
来源：http://stb.redwolf501.top

[G08] 静态方法与属性
来源：http://rhs.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vwh.haohaochexian.top

PHP:  public static function f() {}
来源：http://uzc.zhaomingkeji.xyz

JS:   static f() {}
来源：http://fel.bjfxy.top

TS:   static f(): void {}
来源：http://zay.yj202588.top

Java: static void f() {}
来源：http://tan.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ggd.andypj.xyz

Ruby: def self.f; end
来源：http://yuj.ybcxt.top

C#:   public static void F() {}
来源：http://dui.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://vsp.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://mqx.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://kzd.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://atg.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://ssf.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://wba.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://teh.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fhj.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://cdv.svipenyu.cn

[G10] 访问控制
来源：http://hmp.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://eot.dianchejie.cn

PHP:  public / protected / private
来源：http://crp.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://iyn.hammf.cn

TS:   public / protected / private
来源：http://mon.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://vya.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://ite.yfazqb.com

Ruby: public / protected / private
来源：http://uko.yonumen.top

C#:   public / protected / private / internal
来源：http://qnz.kuanghao11.cn

[G11] getter / setter
来源：http://xvz.andypj.xyz

Py:   @property 与 @x.setter
来源：http://kta.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yuq.aizwys.cn

JS:   get name() { return this._name; }
来源：http://pgn.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://fcm.xuanzx.com

Java: public String getName() { return name; }
来源：http://umt.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bjl.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://djx.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://uyr.zycfv.cn

[G12] 对象转字符串
来源：http://kbi.nanxinkj.top

Py:   def __str__(self): return self.name
来源：http://tat.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qzh.yonumen.top

JS:   toString() { return this.name; }
来源：http://zhr.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://eln.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://bbq.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://ror.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://zes.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://iax.ydjk.org.cn

[G13] 判断对象类型
来源：http://gby.yj20258888.top

Py:   isinstance(u, User)
来源：http://him.nanxuanxn.top

PHP:  $u instanceof User
来源：http://dzc.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://thv.chenjidiqi.icu

TS:   u instanceof User
来源：http://yxt.ydzc1.top

Java: u instanceof User
来源：http://wql.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://jxx.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://hss.epnwcf.com

C#:   u is User
来源：http://ydu.mhx1999.top

[G14] 数据类 / record
来源：http://pjs.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hkz.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://rih.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://aak.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://dwg.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://cjt.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://luu.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://saq.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://dee.ydzc1.top

[G15] 枚举
来源：http://eev.dashuyun.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uoh.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pmh.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xqj.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qmg.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://qoq.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zwi.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://kri.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wcu.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://xon.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tgo.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://ndd.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://noy.jianghu66.top

TS:   Object.entries(obj)
来源：http://dws.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pys.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tnk.fzhhl.top

Ruby: obj.instance_variables
来源：http://yyn.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://wcp.cashguo.top

================================================================================
来源：http://mzf.dianchejie.cn

H. 异常与错误处理
来源：http://jnl.ivvv.top

================================================================================
来源：http://rna.xuanzx.com

[H01] try / catch 基础
来源：http://nmm.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ypb.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vmz.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jec.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blj.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uok.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mpo.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uat.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yrc.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://wbv.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ngx.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yxw.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://mqc.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ksg.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://wsg.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ptt.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vub.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://umr.52xcode.cn

[H03] 主动抛出异常
来源：http://dcu.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://mwz.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bti.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://rwz.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://ptb.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fel.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fei.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wmg.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://ifc.fehbvm.com

[H04] 自定义异常类型
来源：http://qhv.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://ecl.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://kom.havefunace.top

JS:   class MyError extends Error {}
来源：http://ckz.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://wan.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://tgx.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfh.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://sry.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://jml.jianghu66.top

[H05] 捕获特定类型
来源：http://wny.yj20258888.top

Py:   except ValueError as e:
来源：http://mnz.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ckr.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://cqk.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://kik.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://ghk.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://euf.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://ymi.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ner.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://lhx.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://uzj.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://nmx.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://wfq.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yup.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xns.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oqw.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://idi.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://fdo.jinqigufen.top

[H07] 断言
来源：http://wyp.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://rmu.bbcook.cn

PHP:  assert($x > 0);
来源：http://lqz.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://qde.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://mhk.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://cie.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ioy.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ako.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://caj.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://ghy.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://rzl.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kpp.hcnkem.com

JS:   e.message;  e.stack
来源：http://fty.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kvn.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zru.yanxiufei.cn

Go:   err.Error()
来源：http://nin.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://jqq.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://tcy.yonumen.top

[H09] 带错误码的异常
来源：http://chz.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nfb.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://omr.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wta.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wwp.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lci.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tmg.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://rcn.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hmn.tarul.cn

[H10] 资源自动释放
来源：http://twu.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fff.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sxj.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vnx.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rzw.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://alh.ehwqpu.com

Go:   defer f.Close()
来源：http://npp.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dji.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kpi.wangshuangyany.cn

================================================================================
来源：http://vhj.chenjidiqi.icu

I. 正则表达式
来源：http://epj.birdmap.top

================================================================================
来源：http://rzh.fzhhl.top

[I01] 判断是否匹配
来源：http://mci.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uts.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ija.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://siv.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://nxv.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oto.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hcs.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://hvs.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lag.nwbrower.top

[I02] 提取所有匹配
来源：http://jcc.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://iie.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vsd.shzxlz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xwd.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://pvn.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oau.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://suy.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://fjn.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tir.dashuyun.cn

[I03] 提取捕获分组
来源：http://iqy.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bhz.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sox.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xtc.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oqq.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qjx.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://itz.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://egn.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mch.vehdjk.com

[I04] 正则替换
来源：http://xck.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://tjx.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ayx.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://byp.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mgz.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://kap.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://inv.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xjw.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pnr.yonumen.top

[I05] 按正则拆分
来源：http://wrk.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tay.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://feh.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://oiw.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://tis.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://bhi.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ugd.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://kjs.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://her.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zip.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wci.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wze.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wff.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ayy.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://peq.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dqu.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qpz.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tzg.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://wyy.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ssi.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mwe.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fhj.hesvh.cn

TS:   /error/gim
来源：http://gfm.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dah.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wow.meibo888.top

Ruby: s.scan(/error/i)
来源：http://mpy.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fbg.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://ucm.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oyi.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ogi.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uyr.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tkz.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://qmi.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://omi.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://brc.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mqk.meibo888.top

================================================================================
来源：http://zsx.nwbrower.top

J. 日期与时间
来源：http://zqs.sufxvd.cn

================================================================================
来源：http://slv.tianlin.xyz

[J01] 获取当前时间
来源：http://ooq.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aid.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ser.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://zgr.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://bhk.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ifo.sweek.top

Go:   time.Now()
来源：http://fze.sufxvd.cn

Ruby: Time.now
来源：http://dnu.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fbn.snrcjt.cn

[J02] 格式化输出
来源：http://vje.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bji.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xvc.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yvc.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://kbk.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://evp.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gia.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jky.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eiq.yuxming.cn

[J03] 字符串解析为日期
来源：http://sbq.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zjq.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://itq.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://zyq.hesvh.cn


<!-- 参考信息 -->