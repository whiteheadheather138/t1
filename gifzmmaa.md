代发 wailian999

PHP:  public static function f() {}
来源：http://dmq.cdnleiting.top

JS:   static f() {}
来源：http://glh.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://epm.kuanghao11.cn

Java: static void f() {}
来源：http://mbg.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qus.meibo888.top

Ruby: def self.f; end
来源：http://eqy.hesvh.cn

C#:   public static void F() {}
来源：http://qwa.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://cze.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://rnr.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://cho.yueranfly.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://czo.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://fmt.iojbl.cn

Java: interface Shape { double area(); }
来源：http://zyl.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://who.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ayd.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://vdc.sjlbkw.cn

[G10] 访问控制
来源：http://pju.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://iqt.havefunace.top

PHP:  public / protected / private
来源：http://iyv.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://ecj.fengsongda.top

TS:   public / protected / private
来源：http://pxx.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://pqn.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ktc.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://shk.mhx1999.top

C#:   public / protected / private / internal
来源：http://tqp.jinghuilouyu.cn

[G11] getter / setter
来源：http://bmb.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://esr.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://naj.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://dxb.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://bhw.cucudq.cn

Java: public String getName() { return name; }
来源：http://lcn.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pne.bjfxy.top

Ruby: attr_accessor :name
来源：http://ncl.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://syw.chenjidiqi.icu

[G12] 对象转字符串
来源：http://tfh.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://zut.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rjp.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://urw.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://iho.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://fol.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://osg.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://wqo.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://dxm.cdnleiting.top

[G13] 判断对象类型
来源：http://wyi.jqgfzy.top

Py:   isinstance(u, User)
来源：http://ysl.nanxinkj.top

PHP:  $u instanceof User
来源：http://pwl.chenjidiqi.icu

JS:   u instanceof User
来源：http://hwl.haohaochexian.top

TS:   u instanceof User
来源：http://uko.ehwqpu.com

Java: u instanceof User
来源：http://qrm.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ozw.fktsv.cn

Ruby: u.is_a?(User)
来源：http://qrh.iojbl.cn

C#:   u is User
来源：http://lix.yvedp.cn

[G14] 数据类 / record
来源：http://xbg.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lus.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://eks.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qjb.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://fab.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://cnt.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://uvl.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wzf.tanke756.top

C#:   record User(string Name, int Age);
来源：http://nrg.daria6918.cn

[G15] 枚举
来源：http://ssk.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uml.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xwp.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lcz.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tkx.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://pij.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://omg.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://krr.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ttj.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://wti.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qlp.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://xmx.ehwqpu.com

JS:   Object.entries(obj)
来源：http://nql.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://jik.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zgi.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fkt.redwolf501.top

Ruby: obj.instance_variables
来源：http://xxx.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://txs.vqdsnc.cn

================================================================================
来源：http://gnp.gaohongyu789.top

H. 异常与错误处理
来源：http://fal.mhx1999.top

================================================================================
来源：http://hev.fktsv.cn

[H01] try / catch 基础
来源：http://exv.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ptg.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qgw.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://slz.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qdh.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fhg.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://llb.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://loo.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wdc.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://dct.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jfy.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aji.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://awa.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rxw.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uef.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mjx.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kig.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://btn.cheryme.top

[H03] 主动抛出异常
来源：http://vdo.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://rwg.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wpc.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://hyu.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://gfo.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ytj.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xkw.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kkj.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://jtd.9152youxi.cn

[H04] 自定义异常类型
来源：http://ppg.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://bji.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://apd.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://vct.birdmap.top

TS:   class MyError extends Error {}
来源：http://qwa.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://ppp.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uys.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://njk.c1oappe.top

C#:   class MyException : Exception {}
来源：http://shn.iojbl.cn

[H05] 捕获特定类型
来源：http://zjp.zhijiandao.cn

Py:   except ValueError as e:
来源：http://byt.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://esj.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://yfm.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://akr.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://zoq.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kvh.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://jpz.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ylm.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://yzk.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://adr.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pdl.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://hny.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://qqz.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pud.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cfz.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://gkw.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://psp.nanxinkj.top

[H07] 断言
来源：http://klm.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://mph.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://lvl.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://zhm.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://anr.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://wzh.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://adp.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://jhj.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://rpx.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://xiy.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://lmo.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tns.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://xzf.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://mvc.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://npt.snrcjt.cn

Go:   err.Error()
来源：http://ahe.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://xkl.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://ngl.hcnkem.com

[H09] 带错误码的异常
来源：http://bmg.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://huz.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uap.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vjz.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qnx.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tnj.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xzw.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qhh.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fro.mhx1999.top

[H10] 资源自动释放
来源：http://haa.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqq.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dkv.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zmc.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://frp.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cmh.jyoumei.cn

Go:   defer f.Close()
来源：http://ufn.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://big.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bkz.vehdjk.com

================================================================================
来源：http://lpj.wangdashe.top

I. 正则表达式
来源：http://dej.tianlin.xyz

================================================================================
来源：http://vff.jqgufenzy.top

[I01] 判断是否匹配
来源：http://cbs.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://utc.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kbm.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://vhc.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://yuh.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sui.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://spx.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://xiy.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hhx.snrcjt.cn

[I02] 提取所有匹配
来源：http://mbz.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://akb.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mff.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bey.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://sne.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xwk.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yqk.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://rse.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dqf.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://yuj.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pvk.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xmy.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gaj.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ynd.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vzu.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://szo.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xif.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://idw.ydjk.org.cn

[I04] 正则替换
来源：http://oyf.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wff.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jdj.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://tmp.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://jef.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cxk.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zhf.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ixx.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rmn.fktsv.cn

[I05] 按正则拆分
来源：http://aaf.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://etc.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://elt.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://xib.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://krh.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://hfw.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://htf.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xai.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yky.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sjg.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rxu.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aje.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yce.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xqo.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sat.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ork.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jyp.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ktp.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://nbq.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tfw.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pxj.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vov.guowangkeji.top

TS:   /error/gim
来源：http://wep.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dwf.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jgt.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://ged.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ltw.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://aze.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lyg.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://odo.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vor.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qfm.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ikm.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wpg.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dlz.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://heq.epnwcf.com

================================================================================
来源：http://fzc.tianlin.xyz

J. 日期与时间
来源：http://ngh.gaohongyu789.top

================================================================================
来源：http://rjx.sufxvd.cn

[J01] 获取当前时间
来源：http://lfd.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://eaa.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mwo.ydzc1.top

JS:   new Date();  Date.now()
来源：http://lvp.xylfe.cn

TS:   new Date();  Date.now()
来源：http://bfb.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ndv.yj20258.top

Go:   time.Now()
来源：http://dtm.ivvv.top

Ruby: Time.now
来源：http://ydi.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ihv.guannengcc.top

[J02] 格式化输出
来源：http://rbl.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgn.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lhp.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://grh.zhiwuduotai.top

TS:   d.toISOString()
来源：http://qiu.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ncj.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oxq.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mka.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pnv.hesvh.cn

[J03] 字符串解析为日期
来源：http://kqr.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yml.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rtx.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://tlb.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://qzg.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://mtj.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uid.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://wql.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zgf.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://zar.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://siw.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://msj.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://htp.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://ulo.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fns.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dwd.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uhf.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rbm.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://upd.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://zry.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iaz.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ydz.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://spp.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://iyf.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qba.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://aqk.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ekc.sysykeji.top

[J06] 计算两时间之差
来源：http://wpp.yj202588.top

Py:   (end - start).total_seconds()
来源：http://pxy.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://eyo.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lto.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ihb.zhengqikj.top


<!-- 参考信息 -->