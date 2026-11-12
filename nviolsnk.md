代发 wailian999

Ruby: super
来源：http://wxx.zhijiandao.cn

C#:   base.Greet();
来源：http://drp.c1oappe.top

[G08] 静态方法与属性
来源：http://rzs.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mwt.yangfankeji.com

PHP:  public static function f() {}
来源：http://ccn.jiagoushi.top

JS:   static f() {}
来源：http://rwl.0kj1m.cn

TS:   static f(): void {}
来源：http://hah.shanyushiyangtech.top

Java: static void f() {}
来源：http://mbo.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://knv.redwolf501.top

Ruby: def self.f; end
来源：http://rep.9152youxi.cn

C#:   public static void F() {}
来源：http://svp.xinyue.icu

[G09] 接口 / 抽象类
来源：http://flc.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://vyx.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xwk.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://scg.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://yrk.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://fib.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://cnm.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tmo.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://pfv.zhijiandao.cn

[G10] 访问控制
来源：http://did.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://bsw.yuxming.cn

PHP:  public / protected / private
来源：http://fjh.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://rye.dashuyun.cn

TS:   public / protected / private
来源：http://hfe.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://hbj.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cum.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://irj.sxryk.cn

C#:   public / protected / private / internal
来源：http://kin.birdmap.top

[G11] getter / setter
来源：http://amh.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://aev.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ocu.hesvh.cn

JS:   get name() { return this._name; }
来源：http://utn.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://wsn.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://anh.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jgy.iojbl.cn

Ruby: attr_accessor :name
来源：http://hou.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://frd.aibaodan.cn

[G12] 对象转字符串
来源：http://ofu.cashguo.top

Py:   def __str__(self): return self.name
来源：http://pes.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://asx.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://xts.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://jts.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://lzr.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://xem.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://puq.yongpay.top

C#:   public override string ToString() => Name;
来源：http://ilq.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://xvj.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://wyu.vehdjk.com

PHP:  $u instanceof User
来源：http://hjo.zhengqikj.top

JS:   u instanceof User
来源：http://fnn.jlsjyb.cn

TS:   u instanceof User
来源：http://tlz.316326.xyz

Java: u instanceof User
来源：http://uog.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bnm.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://ajd.redwolf501.top

C#:   u is User
来源：http://kxq.jinqigfzy.top

[G14] 数据类 / record
来源：http://oju.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fdv.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://hpv.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bhy.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://xhb.bbcook.cn

Java: record User(String name, int age) {}
来源：http://hfj.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://ahi.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nqf.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://ach.andypj.xyz

[G15] 枚举
来源：http://qqs.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://llm.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pqj.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pbd.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://snl.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://kbp.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bua.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://oyf.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xky.316326.xyz

[G16] 对象转数组 / 字典
来源：http://ahd.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ltp.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://sgl.mhx1999.top

JS:   Object.entries(obj)
来源：http://div.c1oappe.top

TS:   Object.entries(obj)
来源：http://sob.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mze.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qpl.smart0.xyz

Ruby: obj.instance_variables
来源：http://xya.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://cja.xuetiantiany.cn

================================================================================
来源：http://zbs.fengsongda.top

H. 异常与错误处理
来源：http://spj.pengpengdd.cyou

================================================================================
来源：http://hdv.tarul.cn

[H01] try / catch 基础
来源：http://zen.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fyc.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vdf.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bpt.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bys.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gfu.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tfq.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hmc.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zvg.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://dpz.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://lsd.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gcm.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pql.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jjw.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rtc.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://crb.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://olq.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yfo.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://xwg.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://ser.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zfy.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://eht.yj20258.top

TS:   throw new Error("错误信息");
来源：http://drz.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://sco.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://adv.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yve.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://fgr.guowangkeji.top

[H04] 自定义异常类型
来源：http://sit.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://fob.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tkt.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://soj.iojbl.cn

TS:   class MyError extends Error {}
来源：http://eaw.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://vnq.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ugu.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://onh.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://cpe.xylfe.cn

[H05] 捕获特定类型
来源：http://fgj.cucudq.cn

Py:   except ValueError as e:
来源：http://bul.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://inr.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://ytw.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://jgn.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://xtw.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://irv.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://pyi.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cql.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://wqm.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://vnl.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://naq.zhaomingkeji.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://wzf.yanxiufei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ixg.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://whx.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jsw.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://rwn.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://dvf.jqgfzy.top

[H07] 断言
来源：http://buz.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://irq.hcnkem.com

PHP:  assert($x > 0);
来源：http://vkx.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://reo.c1oappe.top

TS:   console.assert(x > 0);
来源：http://ouv.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://fbf.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jla.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://umy.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://cac.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://nkt.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://jon.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yep.tianlin.xyz

JS:   e.message;  e.stack
来源：http://pki.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://uwl.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://efq.shanyushiyangkeji.top

Go:   err.Error()
来源：http://geh.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://hee.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://sru.tanke756.top

[H09] 带错误码的异常
来源：http://dee.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://irv.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vlw.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ugk.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xdn.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sdx.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cwf.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qnn.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sov.ctjpmb.com

[H10] 资源自动释放
来源：http://vtq.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://brw.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jsf.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nql.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yku.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fer.ppjwa.cn

Go:   defer f.Close()
来源：http://sfb.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ngb.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ezz.zhaomingkeji.xyz

================================================================================
来源：http://bpf.jqgfzy.top

I. 正则表达式
来源：http://xve.cqqwz.cn

================================================================================
来源：http://wfw.316326.xyz

[I01] 判断是否匹配
来源：http://qbw.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bsf.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kgm.vehdjk.com

JS:   /\d+/.test(s)
来源：http://qda.vehdjk.com

TS:   /\d+/.test(s)
来源：http://yon.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zue.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bbi.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://xco.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dev.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://hrn.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://tqj.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://odc.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://asx.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://qsc.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ssc.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dik.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://vrs.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wgz.haohaochexian.top

[I03] 提取捕获分组
来源：http://suf.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pud.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rcx.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cfc.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yru.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xxv.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wfi.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://llo.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jem.jinghuilouyu.cn

[I04] 正则替换
来源：http://ymm.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qqi.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xbx.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wuv.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://iuc.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://spj.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fyu.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xso.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://clk.yuxming.cn

[I05] 按正则拆分
来源：http://vau.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xrw.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tcp.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://aif.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://lpw.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://kxw.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ynf.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://foi.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vpd.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yhw.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lcw.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ihd.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://opx.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ime.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://waa.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mji.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aoq.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://isn.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://klr.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fvq.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oft.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oga.fzhhl.top

TS:   /error/gim
来源：http://sdz.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://szn.jinyuanbaomall.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lpl.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://ggk.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dla.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://ygq.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qif.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jxt.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rhc.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwz.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ysg.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kcf.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://crk.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uyv.shangyingyoupin.top

================================================================================
来源：http://aam.xylfe.cn

J. 日期与时间
来源：http://ftw.9152youxi.cn

================================================================================
来源：http://syx.yj202588.top

[J01] 获取当前时间
来源：http://jig.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gek.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mhy.c1oappe.top

JS:   new Date();  Date.now()
来源：http://ubh.hnqzz.top

TS:   new Date();  Date.now()
来源：http://hfn.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yvr.sxryk.cn

Go:   time.Now()
来源：http://gfx.nanxinkj.top

Ruby: Time.now
来源：http://fco.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kyh.chenjidiqi.icu

[J02] 格式化输出
来源：http://faw.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://roi.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lrn.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cjx.gzhubu.top

TS:   d.toISOString()
来源：http://kix.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dit.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://glm.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fxk.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rfs.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://phh.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ims.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gqe.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://vhs.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://ogs.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://hrf.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tuw.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://fso.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uhb.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://oco.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wjy.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fwn.gaohongyu789.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rbn.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zsr.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nkf.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hdo.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pmf.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tuu.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://dvw.ivvv.top

Py:   now + timedelta(days=7)
来源：http://dxy.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hma.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ctn.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xwm.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://zze.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://unc.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://ysd.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://gio.fktsv.cn

[J06] 计算两时间之差
来源：http://tct.smart0.xyz


<!-- 参考信息 -->