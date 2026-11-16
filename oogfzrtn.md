代发 wailian999

JS:   super.greet();
来源：http://dvw.uphjek.com

TS:   super.greet();
来源：http://qny.hfpthk.cn

Java: super.greet();
来源：http://dsi.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jnv.quarkkingdee.top

Ruby: super
来源：http://myi.hnqzz.top

C#:   base.Greet();
来源：http://wrz.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://jxj.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ddf.fzhhl.top

PHP:  public static function f() {}
来源：http://uzr.yonumen.top

JS:   static f() {}
来源：http://zyn.hammf.cn

TS:   static f(): void {}
来源：http://tgv.sjlbkw.cn

Java: static void f() {}
来源：http://paw.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ikf.kuanghao11.cn

Ruby: def self.f; end
来源：http://ukn.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://osf.xylfe.cn

[G09] 接口 / 抽象类
来源：http://owe.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://qwa.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aou.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bnb.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://cpf.cashguo.top

Java: interface Shape { double area(); }
来源：http://irc.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://huu.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lch.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://fed.shanyushiyangtech.top

[G10] 访问控制
来源：http://ckp.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://xmt.zdbjq.cn

PHP:  public / protected / private
来源：http://zfz.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://cor.cucudq.cn

TS:   public / protected / private
来源：http://sct.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://pfj.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://exd.zhixingplan.top

Ruby: public / protected / private
来源：http://xbu.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://bdd.yj202588.top

[G11] getter / setter
来源：http://tis.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://tbv.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://maj.mhx1999.top

JS:   get name() { return this._name; }
来源：http://zde.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://yfu.iojbl.cn

Java: public String getName() { return name; }
来源：http://rpq.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zud.fehbvm.com

Ruby: attr_accessor :name
来源：http://dbo.zycfv.cn

C#:   public string Name { get; set; }
来源：http://rjg.nwbrower.top

[G12] 对象转字符串
来源：http://lsl.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://mmg.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lbz.xylfe.cn

JS:   toString() { return this.name; }
来源：http://oqt.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://fri.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://axw.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://hki.vehdjk.com

Ruby: def to_s; @name; end
来源：http://lka.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://dku.xuanzx.com

[G13] 判断对象类型
来源：http://txo.wangdashe.top

Py:   isinstance(u, User)
来源：http://boi.cheryme.top

PHP:  $u instanceof User
来源：http://xda.tianlin.xyz

JS:   u instanceof User
来源：http://txz.yfazqb.com

TS:   u instanceof User
来源：http://gon.ctjpmb.com

Java: u instanceof User
来源：http://jcl.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xmr.cashguo.top

Ruby: u.is_a?(User)
来源：http://svr.316326.xyz

C#:   u is User
来源：http://rrc.pycfn.com

[G14] 数据类 / record
来源：http://wxy.iojbl.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ykp.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://cui.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://idw.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://laf.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://aio.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://ukl.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vfi.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://uba.xuetiantiany.cn

[G15] 枚举
来源：http://tdb.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vwq.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://bib.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ryo.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lzd.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://xvn.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yuq.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://tmj.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dyp.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://hxq.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oei.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://ore.hfpthk.cn

JS:   Object.entries(obj)
来源：http://qei.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://bjp.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dfl.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fgz.cqqwz.cn

Ruby: obj.instance_variables
来源：http://pjx.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://avg.xylfe.cn

================================================================================
来源：http://wkj.yangfankeji.com

H. 异常与错误处理
来源：http://mqt.yuanzhike.top

================================================================================
来源：http://anp.hongshengwenyu.top

[H01] try / catch 基础
来源：http://nex.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lrs.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bry.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hyr.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pkw.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jva.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wjl.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mrf.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qzd.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://ctj.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://hgq.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rbf.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sto.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://hml.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://grt.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qhc.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ltz.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fqk.kuanghao11.cn

[H03] 主动抛出异常
来源：http://dna.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://oao.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rlc.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://zfr.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://bqo.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wpz.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jzj.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jqy.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://fym.hnqzz.top

[H04] 自定义异常类型
来源：http://rwm.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://iwa.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jtb.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://pua.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://izn.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://zqh.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fgb.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://zfn.cheryme.top

C#:   class MyException : Exception {}
来源：http://dhq.zhoulong.xyz

[H05] 捕获特定类型
来源：http://dyy.smart0.xyz

Py:   except ValueError as e:
来源：http://apu.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pqr.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://uck.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://bnr.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://thw.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ljt.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://dvu.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pah.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://gdc.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://xfz.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://jtc.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://xij.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://gbw.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ryv.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pyp.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://jzt.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://hec.yvedp.cn

[H07] 断言
来源：http://lxf.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://ttx.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://wvo.tanke756.top

JS:   console.assert(x > 0);
来源：http://swf.fktsv.cn

TS:   console.assert(x > 0);
来源：http://msl.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://jgf.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eei.shanyushiyangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://iwi.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://jvz.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://dci.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://rph.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uhr.tarul.cn

JS:   e.message;  e.stack
来源：http://zvr.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cgj.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mfg.epnwcf.com

Go:   err.Error()
来源：http://etu.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://lgj.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://vaf.hfpthk.cn

[H09] 带错误码的异常
来源：http://yja.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uvb.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eum.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://unk.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yji.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hug.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eft.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://jwo.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://flx.birdmap.top

[H10] 资源自动释放
来源：http://ghs.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qus.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://imu.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://avt.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mmh.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://llu.havefunace.top

Go:   defer f.Close()
来源：http://guo.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://glk.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bat.chenlongwang.top

================================================================================
来源：http://kiz.shuidangran.top

I. 正则表达式
来源：http://brj.bjfxy.top

================================================================================
来源：http://moz.zhixingplan.top

[I01] 判断是否匹配
来源：http://isk.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://etr.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://btr.hnqzz.top

JS:   /\d+/.test(s)
来源：http://iha.xylfe.cn

TS:   /\d+/.test(s)
来源：http://yum.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zvc.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tbs.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://dtu.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vbm.zhoulong.xyz

[I02] 提取所有匹配
来源：http://sek.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://plw.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qdg.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tsd.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://fms.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://imk.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fof.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://hqv.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://elv.yj20258888.top

[I03] 提取捕获分组
来源：http://nbh.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rpx.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://klt.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lgz.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ldi.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kpg.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bpr.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yyu.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lyz.quarkkingdee.top

[I04] 正则替换
来源：http://avz.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mlz.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dlm.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nub.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://thy.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://ria.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gbp.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fjq.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kpt.zhoulong.xyz

[I05] 按正则拆分
来源：http://dgx.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aja.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xjp.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://hzw.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://vmo.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://xqd.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qbq.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://rgo.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://swk.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wqa.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rkh.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://akr.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zya.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://esx.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uai.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tqp.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://voq.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hiv.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://ctn.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://czm.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xnf.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pjd.shuidangran.top

TS:   /error/gim
来源：http://itr.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xgl.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://emi.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://seu.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bch.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://vgy.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rhx.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dym.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ydh.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycs.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cqk.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wbo.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ucr.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://utj.jinqigfzy.top

================================================================================
来源：http://gje.gzhubu.top

J. 日期与时间
来源：http://pgb.zhengqikj.top

================================================================================
来源：http://jjx.wangdashe.top

[J01] 获取当前时间
来源：http://ekg.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bty.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sya.xziqi.cn

JS:   new Date();  Date.now()
来源：http://sxz.yongpay.top

TS:   new Date();  Date.now()
来源：http://voh.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xrk.jinyuanbaomall.cn

Go:   time.Now()
来源：http://dse.birdmap.top

Ruby: Time.now
来源：http://kys.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dkh.tianlin.xyz

[J02] 格式化输出
来源：http://obn.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qjj.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nzj.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://whp.wangshuangyany.cn

TS:   d.toISOString()
来源：http://ikz.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yek.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cla.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqi.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://slo.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://tvj.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dhn.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vpu.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://rww.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://lxs.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bjq.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pqi.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://lzi.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cuu.birdmap.top

[J04] 时间戳与日期互转
来源：http://xwq.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uby.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qst.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ztm.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qqi.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vcj.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qiz.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sgf.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vjz.cheryme.top

[J05] 时间加减（加 7 天）
来源：http://whj.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://ouh.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://xzs.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tcu.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oxb.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://ess.jinyuanbaomall.cn


<!-- 参考信息 -->