代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://nok.wangshuangyany.cn

[G07] 调用父类方法
来源：http://hfg.vehdjk.com

Py:   super().greet()
来源：http://hco.cashguo.top

PHP:  parent::greet();
来源：http://uyi.aibaodan.cn

JS:   super.greet();
来源：http://vce.xuanzx.com

TS:   super.greet();
来源：http://tik.sysykeji.top

Java: super.greet();
来源：http://zet.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kwf.zhixingplan.top

Ruby: super
来源：http://iab.nanxinkj.top

C#:   base.Greet();
来源：http://nik.pycfn.com

[G08] 静态方法与属性
来源：http://jzb.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pom.zhoulong.xyz

PHP:  public static function f() {}
来源：http://ktk.dashuyun.cn

JS:   static f() {}
来源：http://xlv.sysykeji.top

TS:   static f(): void {}
来源：http://xxk.jinqigufen.top

Java: static void f() {}
来源：http://anh.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://izz.snrcjt.cn

Ruby: def self.f; end
来源：http://ywu.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://vyu.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://duj.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://eew.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cst.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://trw.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://lsa.sweek.top

Java: interface Shape { double area(); }
来源：http://wcl.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://qdd.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uvi.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://xle.jyoumei.cn

[G10] 访问控制
来源：http://lhm.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://rbw.yj20258.top

PHP:  public / protected / private
来源：http://kvw.epnwcf.com

JS:   #private 字段；其余公开
来源：http://ifs.kuanghao11.cn

TS:   public / protected / private
来源：http://mxy.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://pmz.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sbs.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://kzw.nwbrower.top

C#:   public / protected / private / internal
来源：http://rno.tian-w.cn

[G11] getter / setter
来源：http://mxf.tanke756.top

Py:   @property 与 @x.setter
来源：http://lti.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ine.zycfv.cn

JS:   get name() { return this._name; }
来源：http://wrr.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://rve.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://pge.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rbi.shzxlz.cn

Ruby: attr_accessor :name
来源：http://kvs.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://yyq.yuanzhike.top

[G12] 对象转字符串
来源：http://xzi.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://anj.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kfd.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://abn.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://gae.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://hye.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://puv.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://gpp.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://kdw.yonumen.top

[G13] 判断对象类型
来源：http://bmh.ehwqpu.com

Py:   isinstance(u, User)
来源：http://oxp.xinyue.icu

PHP:  $u instanceof User
来源：http://ffb.sweek.top

JS:   u instanceof User
来源：http://nuj.shzxlz.cn

TS:   u instanceof User
来源：http://vpx.wangdashe.top

Java: u instanceof User
来源：http://nym.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jzy.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://vta.guannengcc.top

C#:   u is User
来源：http://udg.cashguo.top

[G14] 数据类 / record
来源：http://xab.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hjt.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://bpf.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://cwx.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://cat.birdmap.top

Java: record User(String name, int age) {}
来源：http://lub.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://xiz.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qvw.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://ijp.ydzc1.top

[G15] 枚举
来源：http://tap.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yaw.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kan.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nmj.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://emk.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://qyk.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uoe.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://clb.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sti.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://xwi.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xnq.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://urg.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://qzc.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://vrk.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qcj.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ugt.pycfn.com

Ruby: obj.instance_variables
来源：http://fkc.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://ehq.hammf.cn

================================================================================
来源：http://maz.jianghu66.top

H. 异常与错误处理
来源：http://bhq.yfazqb.com

================================================================================
来源：http://ydt.chenjidiqi.icu

[H01] try / catch 基础
来源：http://gfe.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lnb.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rzm.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jpw.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gum.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pzs.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cxf.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://crf.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tzb.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://hmm.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://zjk.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wef.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rpc.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ybp.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://pyn.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lco.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rpc.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nqd.yonumen.top

[H03] 主动抛出异常
来源：http://qzc.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://jki.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xyc.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://rrh.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://gik.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lhy.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fku.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rck.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://geq.gogol.net.cn

[H04] 自定义异常类型
来源：http://wac.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://wsq.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://ibr.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://gvx.zycfv.cn

TS:   class MyError extends Error {}
来源：http://jsh.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://izp.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ton.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://fjh.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://hcf.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://fzw.bbcook.cn

Py:   except ValueError as e:
来源：http://xox.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dzc.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://mvr.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://xzd.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://ifa.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pfx.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://sdd.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dfk.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://mqt.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://qok.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://zcp.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gaz.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wop.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ymh.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uhp.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://wiw.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://cri.chenjidiqi.icu

[H07] 断言
来源：http://ksw.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://rjr.tian-w.cn

PHP:  assert($x > 0);
来源：http://tam.316326.xyz

JS:   console.assert(x > 0);
来源：http://fmv.tarul.cn

TS:   console.assert(x > 0);
来源：http://qnb.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://kwe.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dva.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://sya.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://bsf.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://kji.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://juw.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xjq.chenlongwang.top

JS:   e.message;  e.stack
来源：http://jzj.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xdw.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bme.wangdashe.top

Go:   err.Error()
来源：http://jvs.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://hck.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://beu.ydjk.org.cn

[H09] 带错误码的异常
来源：http://phf.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oqf.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://enh.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oxv.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nmp.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hrl.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jue.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://fkc.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lqo.cashguo.top

[H10] 资源自动释放
来源：http://ukb.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ulw.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gdl.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qzo.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cxu.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rym.vehdjk.com

Go:   defer f.Close()
来源：http://few.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://efu.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gci.chenlongwang.top

================================================================================
来源：http://xjk.havefunace.top

I. 正则表达式
来源：http://fox.hywenlv.cn

================================================================================
来源：http://fhl.quarkkingdee.top

[I01] 判断是否匹配
来源：http://omn.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vdz.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://guw.sweek.top

JS:   /\d+/.test(s)
来源：http://zdq.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://qpv.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uxt.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tml.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://ckz.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qjt.nanxuanxn.top

[I02] 提取所有匹配
来源：http://rwe.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://rib.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iiu.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vpn.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://zpo.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://znx.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ygn.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://ydg.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cvc.mhx1999.top

[I03] 提取捕获分组
来源：http://puc.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iwz.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gdz.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ddz.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vhh.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ljb.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mit.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zye.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wwh.fehbvm.com

[I04] 正则替换
来源：http://nix.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vqu.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ojg.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://yzz.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://gbh.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://wee.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://yyf.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qzi.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aqw.ehwqpu.com

[I05] 按正则拆分
来源：http://fgt.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eql.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://biz.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://oot.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://fbp.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://hlk.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lcw.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://bln.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qxd.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pyo.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uwo.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gtn.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpt.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsg.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aev.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xbu.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kua.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dcc.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://fha.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zsv.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://neq.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pho.zhiwuduotai.top

TS:   /error/gim
来源：http://ljj.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cop.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zwy.tarul.cn

Ruby: s.scan(/error/i)
来源：http://ihg.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tfq.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://hlu.fzhhl.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://isw.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kwr.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ypn.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mka.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://zfl.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wvo.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pzf.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dzb.wangshuangyany.cn

================================================================================
来源：http://skd.meibo888.top

J. 日期与时间
来源：http://odo.andypj.xyz

================================================================================
来源：http://wwo.hesvh.cn

[J01] 获取当前时间
来源：http://lph.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qob.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mfa.meibo888.top

JS:   new Date();  Date.now()
来源：http://plf.xuanzx.com

TS:   new Date();  Date.now()
来源：http://qxx.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fxh.wangshuangyany.cn

Go:   time.Now()
来源：http://sqw.epnwcf.com

Ruby: Time.now
来源：http://izs.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vib.vehdjk.com

[J02] 格式化输出
来源：http://ywp.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gvw.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://koo.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yxm.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://tqt.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ase.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qif.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gry.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pin.wangdashe.top

[J03] 字符串解析为日期
来源：http://zhv.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fzo.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ziq.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://wxe.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://bxn.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hkm.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ufo.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://drm.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fjm.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://rbg.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://spg.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://api.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pxf.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rdl.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pca.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://otb.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jfx.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cus.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://muo.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://fbz.bbcook.cn


<!-- 参考信息 -->