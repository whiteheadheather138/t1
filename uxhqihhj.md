代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://isv.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://sbe.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ake.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://usl.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://ahz.sjlbkw.cn

[G07] 调用父类方法
来源：http://cfq.fanxiaobao.xyz

Py:   super().greet()
来源：http://qwv.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://rgn.gzhubu.top

JS:   super.greet();
来源：http://gzk.gzhubu.top

TS:   super.greet();
来源：http://gkf.jyoumei.cn

Java: super.greet();
来源：http://lud.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kno.zhijiandao.cn

Ruby: super
来源：http://ept.uphjek.com

C#:   base.Greet();
来源：http://ets.pycfn.com

[G08] 静态方法与属性
来源：http://mlv.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vlm.nwbrower.top

PHP:  public static function f() {}
来源：http://pzc.haohaochexian.top

JS:   static f() {}
来源：http://aee.gotoacloud.top

TS:   static f(): void {}
来源：http://zij.hysaishi.cn

Java: static void f() {}
来源：http://zuw.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lwn.shanyushiyangkeji.top

Ruby: def self.f; end
来源：http://zxh.pengpengdd.cyou

C#:   public static void F() {}
来源：http://ufs.yj202588.top

[G09] 接口 / 抽象类
来源：http://tif.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://loe.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://nih.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://unp.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://nrs.sxryk.cn

Java: interface Shape { double area(); }
来源：http://pjh.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://nrm.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jym.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://roc.cdnleiting.top

[G10] 访问控制
来源：http://tdw.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://tgf.shangyingyoupin.top

PHP:  public / protected / private
来源：http://iev.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://wnt.redwolf501.top

TS:   public / protected / private
来源：http://jzp.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://pji.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nki.epnwcf.com

Ruby: public / protected / private
来源：http://apr.ivvv.top

C#:   public / protected / private / internal
来源：http://qmd.zhixingplan.top

[G11] getter / setter
来源：http://cut.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://xzg.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ubf.xylfe.cn

JS:   get name() { return this._name; }
来源：http://stz.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://ymo.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://klp.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pai.cashguo.top

Ruby: attr_accessor :name
来源：http://ryh.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://eaw.jlsjyb.cn

[G12] 对象转字符串
来源：http://bmj.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://sxa.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cep.yuxming.cn

JS:   toString() { return this.name; }
来源：http://dez.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://wpl.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://hkg.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://urb.cucudq.cn

Ruby: def to_s; @name; end
来源：http://wai.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://jgy.316326.xyz

[G13] 判断对象类型
来源：http://pyd.xylfe.cn

Py:   isinstance(u, User)
来源：http://vhs.cdnleiting.top

PHP:  $u instanceof User
来源：http://oiw.chenlongwang.top

JS:   u instanceof User
来源：http://gfj.svipenyu.cn

TS:   u instanceof User
来源：http://upl.zhengqikj.top

Java: u instanceof User
来源：http://arr.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uxv.tarul.cn

Ruby: u.is_a?(User)
来源：http://eln.zhoulong.xyz

C#:   u is User
来源：http://wfq.316326.xyz

[G14] 数据类 / record
来源：http://cdw.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://chp.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://rrq.andypj.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://amq.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://cmx.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://sxz.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://nvm.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jfa.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://wrq.ybcxt.top

[G15] 枚举
来源：http://pii.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://otj.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qvr.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yru.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eww.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://sza.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nto.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://kuy.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pif.meibo888.top

[G16] 对象转数组 / 字典
来源：http://rab.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fat.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://zmy.shzxlz.cn

JS:   Object.entries(obj)
来源：http://gqu.zhixingplan.top

TS:   Object.entries(obj)
来源：http://yri.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ujh.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://btg.fehbvm.com

Ruby: obj.instance_variables
来源：http://aem.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ytb.shanyushiyangtech.top

================================================================================
来源：http://mwm.yuxming.cn

H. 异常与错误处理
来源：http://zsf.zhoulong.xyz

================================================================================
来源：http://fxn.sweek.top

[H01] try / catch 基础
来源：http://ztg.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://utm.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cyn.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hat.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xyc.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://crc.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vvu.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bid.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zcj.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://rwv.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aah.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vrd.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lzg.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xvv.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://vzj.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://yhm.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fvk.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yvt.yueranfly.top

[H03] 主动抛出异常
来源：http://imi.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://esm.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yhb.hammf.cn

JS:   throw new Error("错误信息");
来源：http://agu.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://iwh.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://lza.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://klf.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rly.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pvi.nanxuanxn.top

[H04] 自定义异常类型
来源：http://yrv.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://dvt.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kwb.cheryme.top

JS:   class MyError extends Error {}
来源：http://kxo.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://lif.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://pph.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vgh.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://cuz.fehbvm.com

C#:   class MyException : Exception {}
来源：http://jhz.fengsongda.top

[H05] 捕获特定类型
来源：http://zkq.quarkkingdee.top

Py:   except ValueError as e:
来源：http://tie.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://grw.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://wut.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://hzy.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://tmj.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dll.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://orr.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eii.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://pzj.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://div.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lcu.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://iry.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://jpl.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oah.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vpt.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://dzz.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://nci.jinqigfzy.top

[H07] 断言
来源：http://yqt.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://cyy.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://abf.mhx1999.top

JS:   console.assert(x > 0);
来源：http://zth.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://ttc.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://pms.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zrk.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yzp.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://gkq.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://bpw.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://ptt.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ull.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://zli.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ujc.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bxb.jqgfzy.top

Go:   err.Error()
来源：http://vuq.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://tri.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://sbi.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://qww.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tjz.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qmc.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pgl.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kpj.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://btg.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://clv.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://gep.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nbh.redwolf501.top

[H10] 资源自动释放
来源：http://laf.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wvw.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://upl.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gog.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bka.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tye.yanxiufei.cn

Go:   defer f.Close()
来源：http://eoe.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ftv.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bsa.hesvh.cn

================================================================================
来源：http://stb.jinqigufen.top

I. 正则表达式
来源：http://myk.sweek.top

================================================================================
来源：http://cus.gzhubu.top

[I01] 判断是否匹配
来源：http://zva.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vkq.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://aqr.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://gmq.bbcook.cn

TS:   /\d+/.test(s)
来源：http://vtz.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wra.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bxo.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://gck.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yem.ppjwa.cn

[I02] 提取所有匹配
来源：http://hwx.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://rsa.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dlu.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://crp.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://adv.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dzh.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jua.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://gmg.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xfh.fehbvm.com

[I03] 提取捕获分组
来源：http://gzx.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqb.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dce.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bqi.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qlh.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dms.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jmp.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gvk.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://edh.iojbl.cn

[I04] 正则替换
来源：http://tyq.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://six.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vob.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://jrj.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://yzd.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://kts.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uxt.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ars.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://juy.zhengqikj.top

[I05] 按正则拆分
来源：http://sip.kuanghao11.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gzh.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ibn.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://qfe.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://gmu.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://ury.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://htx.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://rdx.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fxv.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fmn.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ael.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uar.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qir.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://row.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qut.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://unw.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zfu.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tzp.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://tli.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://stn.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jnu.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dcv.haohaochexian.top

TS:   /error/gim
来源：http://rbu.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://les.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xho.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://dzq.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rfq.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://aud.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ael.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yxm.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://otm.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://via.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://avj.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dzm.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dse.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nhg.chenjidiqi.icu

================================================================================
来源：http://fbs.ybcxt.top

J. 日期与时间
来源：http://zig.daria6918.cn

================================================================================
来源：http://ava.ehwqpu.com

[J01] 获取当前时间
来源：http://ldr.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://frf.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hoh.yuxming.cn

JS:   new Date();  Date.now()
来源：http://coy.aizwys.cn

TS:   new Date();  Date.now()
来源：http://tis.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ziu.zdqjudy.top

Go:   time.Now()
来源：http://wqu.shanyushiyangkeji.top

Ruby: Time.now
来源：http://fja.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hyb.chenjidiqi.icu

[J02] 格式化输出
来源：http://cpj.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://des.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rkq.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ypk.feifeiyinyue.top

TS:   d.toISOString()
来源：http://wtf.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jgk.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xtb.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zjz.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jbd.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://gbx.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://osa.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bsp.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://lxi.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://stm.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://foo.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zsn.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://dtt.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yhe.hnqzz.top

[J04] 时间戳与日期互转
来源：http://psf.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ges.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ovz.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vhe.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tdi.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kvm.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xqj.andypj.xyz


<!-- 参考信息 -->