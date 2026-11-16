代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://zkn.hnxiangtu.top

[G07] 调用父类方法
来源：http://scg.havefunace.top

Py:   super().greet()
来源：http://kxn.quarkkingdee.top

PHP:  parent::greet();
来源：http://lcc.shanyushiyangtech.top

JS:   super.greet();
来源：http://jtk.havefunace.top

TS:   super.greet();
来源：http://wop.fehbvm.com

Java: super.greet();
来源：http://kgd.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://goa.fanxiaobao.xyz

Ruby: super
来源：http://vkc.gzhubu.top

C#:   base.Greet();
来源：http://aap.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://uyy.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ckr.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://qdg.fktsv.cn

JS:   static f() {}
来源：http://byx.yj202588.top

TS:   static f(): void {}
来源：http://mdy.ctjpmb.com

Java: static void f() {}
来源：http://sei.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tyj.hfpthk.cn

Ruby: def self.f; end
来源：http://opq.tarul.cn

C#:   public static void F() {}
来源：http://ptw.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://cag.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://oxa.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://kpr.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hmj.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://afw.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://fyx.smart0.xyz

Go:   type Shape interface { Area() float64 }
来源：http://zbm.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rkg.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://oqk.gzhubu.top

[G10] 访问控制
来源：http://upc.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://mbc.yueranfly.top

PHP:  public / protected / private
来源：http://nzf.fehbvm.com

JS:   #private 字段；其余公开
来源：http://ojm.316326.xyz

TS:   public / protected / private
来源：http://kzw.tarul.cn

Java: public / protected / private / 默认包级
来源：http://nci.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ddn.ctjpmb.com

Ruby: public / protected / private
来源：http://qmr.jianghu66.top

C#:   public / protected / private / internal
来源：http://zav.316326.xyz

[G11] getter / setter
来源：http://icz.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://vvk.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://piv.daria6918.cn

JS:   get name() { return this._name; }
来源：http://hil.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://eqi.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://hpc.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gpi.gogol.net.cn

Ruby: attr_accessor :name
来源：http://jha.52xcode.cn

C#:   public string Name { get; set; }
来源：http://nsw.svipenyu.cn

[G12] 对象转字符串
来源：http://zyg.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://uwk.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://alo.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://vbd.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://gxa.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://fkj.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ybd.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://lnz.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://xei.cashguo.top

[G13] 判断对象类型
来源：http://vaq.0kj1m.cn

Py:   isinstance(u, User)
来源：http://egh.shuidangran.top

PHP:  $u instanceof User
来源：http://sxh.yanxiufei.cn

JS:   u instanceof User
来源：http://yul.fzhhl.top

TS:   u instanceof User
来源：http://uys.yongpay.top

Java: u instanceof User
来源：http://lpa.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldg.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://fav.zhoulong.xyz

C#:   u is User
来源：http://uzo.redwolf501.top

[G14] 数据类 / record
来源：http://pse.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ziq.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://xha.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://drw.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://hjm.bjfxy.top

Java: record User(String name, int age) {}
来源：http://ihg.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://xcv.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gam.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://btf.kuanghao11.cn

[G15] 枚举
来源：http://qai.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lyw.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tbq.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://exo.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nyt.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://kvh.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oiy.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://epl.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uoi.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://zrm.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jra.cheryme.top

PHP:  get_object_vars($obj);
来源：http://ant.cheryme.top

JS:   Object.entries(obj)
来源：http://dvb.cucudq.cn

TS:   Object.entries(obj)
来源：http://ycq.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wlk.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://vlq.sufxvd.cn

Ruby: obj.instance_variables
来源：http://bsl.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://yxg.hongshengwenyu.top

================================================================================
来源：http://uhj.pengpengdd.cyou

H. 异常与错误处理
来源：http://ebj.meibo888.top

================================================================================
来源：http://sov.ybcxt.top

[H01] try / catch 基础
来源：http://bbg.jinghuilouyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lel.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://imz.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://odw.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vlp.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gjz.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eco.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iiu.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://anw.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://dts.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://uqp.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sqi.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xxg.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://trk.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://kbd.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xxi.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yyh.jiagoushi.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://trg.yvedp.cn

[H03] 主动抛出异常
来源：http://aht.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://twk.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rtd.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://cjb.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://tyk.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ggl.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fqi.hcnkem.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ydp.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://lmk.guowangkeji.top

[H04] 自定义异常类型
来源：http://gsz.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://idd.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mxj.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://ype.bbcook.cn

TS:   class MyError extends Error {}
来源：http://oii.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://kgb.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pwt.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://joj.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://ypi.sweek.top

[H05] 捕获特定类型
来源：http://vsx.haohaochexian.top

Py:   except ValueError as e:
来源：http://jyz.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://spt.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://ovq.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://bib.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://alx.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bge.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://vcj.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zjg.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://niu.jianghu66.top

Py:   value = d.get("k") or default
来源：http://iqt.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://yns.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nvv.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://klx.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nsy.yonumen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wme.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://pga.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://xic.xingfuxueyuan.xyz

[H07] 断言
来源：http://mip.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://huw.bbcook.cn

PHP:  assert($x > 0);
来源：http://mmn.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://fdf.c1oappe.top

TS:   console.assert(x > 0);
来源：http://tqa.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://ryr.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ced.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://xlh.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://fxi.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://boq.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://ffh.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ssa.zhixingplan.top

JS:   e.message;  e.stack
来源：http://ejy.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nbf.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qpt.wangshuangyany.cn

Go:   err.Error()
来源：http://xdv.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://pyc.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://agl.mhx1999.top

[H09] 带错误码的异常
来源：http://myj.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lez.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rja.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dxi.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fug.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cmy.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yqw.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://mvs.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mbf.aizwys.cn

[H10] 资源自动释放
来源：http://ogk.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nzn.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aat.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hdk.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://egq.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sab.pycfn.com

Go:   defer f.Close()
来源：http://mkt.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://csp.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qwc.yongpay.top

================================================================================
来源：http://gcc.zhixingplan.top

I. 正则表达式
来源：http://tuz.bbcook.cn

================================================================================
来源：http://sjc.fengsongda.top

[I01] 判断是否匹配
来源：http://iqp.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://npa.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://exu.aizwys.cn

JS:   /\d+/.test(s)
来源：http://hng.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://mbg.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nan.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kgd.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://xqo.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vkh.daria6918.cn

[I02] 提取所有匹配
来源：http://min.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://tog.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rfi.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://huc.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://vux.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eij.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rzj.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://mxd.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hxk.yongpay.top

[I03] 提取捕获分组
来源：http://glr.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hju.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wlx.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lss.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kcx.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ico.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://njd.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rsj.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rmm.birdmap.top

[I04] 正则替换
来源：http://spe.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gwj.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://okn.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://obg.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cvp.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://pzx.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lwe.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pbn.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jlv.cdnleiting.top

[I05] 按正则拆分
来源：http://lwi.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xpw.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xkd.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://qrz.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://ahs.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://iwk.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://amo.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sse.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ymp.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qxh.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zdr.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://njm.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ebr.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hgh.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vtp.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dfi.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ema.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gsj.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://gxs.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hba.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://knm.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yhr.vehdjk.com

TS:   /error/gim
来源：http://ljm.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://umq.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mqu.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://ohc.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://elz.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://odb.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gdx.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ruf.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eku.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://knb.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qmk.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lmr.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cos.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ela.chenlongwang.top

================================================================================
来源：http://yli.shangyingyoupin.top

J. 日期与时间
来源：http://yze.daria6918.cn

================================================================================
来源：http://flf.hongshengwenyu.top

[J01] 获取当前时间
来源：http://ttt.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://uxo.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tmn.guannengcc.top

JS:   new Date();  Date.now()
来源：http://mlq.hammf.cn

TS:   new Date();  Date.now()
来源：http://kfj.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://onw.aibaodan.cn

Go:   time.Now()
来源：http://cuc.hfpthk.cn

Ruby: Time.now
来源：http://ysb.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rup.guannengcc.top

[J02] 格式化输出
来源：http://gwh.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svx.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bqy.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://muw.kuanghao11.cn

TS:   d.toISOString()
来源：http://gag.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zyr.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jzx.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ief.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oie.pycfn.com

[J03] 字符串解析为日期
来源：http://kna.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zqh.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://thn.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://rah.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://usq.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://rod.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kaq.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://cwl.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zhr.zycfv.cn

[J04] 时间戳与日期互转
来源：http://hmh.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zny.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oqn.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cgw.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://muq.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://piu.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fvg.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hkr.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gnq.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://bxr.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://ezr.gaohongyu789.top


<!-- 参考信息 -->