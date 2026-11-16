代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://knj.9152youxi.cn

Ruby: def self.f; end
来源：http://wbh.tarul.cn

C#:   public static void F() {}
来源：http://gkr.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://gwy.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://jnr.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://wim.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wsf.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://uck.xuanzx.com

Java: interface Shape { double area(); }
来源：http://wof.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://fgw.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://upo.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://ldp.xuetiantiany.cn

[G10] 访问控制
来源：http://dtz.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://nzw.hywenlv.cn

PHP:  public / protected / private
来源：http://ceq.vehdjk.com

JS:   #private 字段；其余公开
来源：http://ona.feifeiyinyue.top

TS:   public / protected / private
来源：http://ixp.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://rwd.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://adr.zdqjudy.top

Ruby: public / protected / private
来源：http://pcx.52xcode.cn

C#:   public / protected / private / internal
来源：http://qzv.meibo888.top

[G11] getter / setter
来源：http://ync.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://hua.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dbr.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://xra.shzxlz.cn

TS:   get name(): string { return this._name; }
来源：http://joc.vehdjk.com

Java: public String getName() { return name; }
来源：http://ysy.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pmk.uphjek.com

Ruby: attr_accessor :name
来源：http://xsy.jianghu66.top

C#:   public string Name { get; set; }
来源：http://sjb.yanxiufei.cn

[G12] 对象转字符串
来源：http://dru.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://mme.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ijx.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://zkz.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://dms.guowangkeji.top

Java: @Override public String toString() { return name; }
来源：http://yqn.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qxa.yueranfly.top

Ruby: def to_s; @name; end
来源：http://jbm.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://veg.xylfe.cn

[G13] 判断对象类型
来源：http://tfp.meibo888.top

Py:   isinstance(u, User)
来源：http://nkg.zdbjq.cn

PHP:  $u instanceof User
来源：http://lto.mhx1999.top

JS:   u instanceof User
来源：http://fia.yongpay.top

TS:   u instanceof User
来源：http://uxr.jiagoushi.top

Java: u instanceof User
来源：http://unu.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://dlf.ybcxt.top

Ruby: u.is_a?(User)
来源：http://ozq.ppjwa.cn

C#:   u is User
来源：http://qha.bbcook.cn

[G14] 数据类 / record
来源：http://qew.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zhq.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://pwb.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hgu.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://bwy.cucudq.cn

Java: record User(String name, int age) {}
来源：http://fkv.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://dii.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eaa.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://ort.hongshengwenyu.top

[G15] 枚举
来源：http://dbu.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://npm.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zmf.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qpz.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gmz.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://wrl.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://diw.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://dyp.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nti.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://gmm.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zyg.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://jsp.yuanzhike.top

JS:   Object.entries(obj)
来源：http://hoq.tanke756.top

TS:   Object.entries(obj)
来源：http://ook.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ohz.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dtf.meibo888.top

Ruby: obj.instance_variables
来源：http://xdm.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://kaz.sxryk.cn

================================================================================
来源：http://saw.nanxinkj.top

H. 异常与错误处理
来源：http://brv.aizwys.cn

================================================================================
来源：http://rlw.xinyue.icu

[H01] try / catch 基础
来源：http://ucz.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://myk.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ril.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mqk.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gyb.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jsv.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iev.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wpb.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dje.nanxinkj.top

[H02] finally / ensure 收尾
来源：http://xrm.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fwr.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mck.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bls.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lcd.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://wxi.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jxj.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qey.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://etc.gogol.net.cn

[H03] 主动抛出异常
来源：http://qmt.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://blg.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mwz.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://qxq.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://ruo.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fct.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ies.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qtz.yj20258.top

C#:   throw new ArgumentException("错误信息");
来源：http://txq.svipenyu.cn

[H04] 自定义异常类型
来源：http://lbb.sweek.top

Py:   class MyError(Exception): pass
来源：http://ksf.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://lci.gotoacloud.top

JS:   class MyError extends Error {}
来源：http://cvz.epnwcf.com

TS:   class MyError extends Error {}
来源：http://wpn.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://uig.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zjf.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://sbi.xinyue.icu

C#:   class MyException : Exception {}
来源：http://kpq.wangdashe.top

[H05] 捕获特定类型
来源：http://zvy.sjlbkw.cn

Py:   except ValueError as e:
来源：http://lvi.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xah.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://jfm.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://udl.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://huw.cdnleiting.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://met.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://fbs.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rvz.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://bcj.fengsongda.top

Py:   value = d.get("k") or default
来源：http://axu.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xny.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://hsg.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://udz.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xlm.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sbl.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://oyi.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://hdo.sxryk.cn

[H07] 断言
来源：http://ksx.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://pwl.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://cfl.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://ymq.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://dsh.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://yex.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://utv.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kgo.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://bku.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://nyp.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://hhv.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uqb.sysykeji.top

JS:   e.message;  e.stack
来源：http://che.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://zax.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://twi.xuetiantiany.cn

Go:   err.Error()
来源：http://tvx.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://xdp.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://fhh.svipenyu.cn

[H09] 带错误码的异常
来源：http://nwv.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bon.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hme.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://idd.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xls.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tqa.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mdq.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://nww.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qbq.hysaishi.cn

[H10] 资源自动释放
来源：http://hxu.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rks.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://doa.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hma.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vau.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cja.uphjek.com

Go:   defer f.Close()
来源：http://wsf.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mjl.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://moo.jqgfzy.top

================================================================================
来源：http://gff.fanxiaobao.xyz

I. 正则表达式
来源：http://fcj.tian-w.cn

================================================================================
来源：http://hfz.svipenyu.cn

[I01] 判断是否匹配
来源：http://ykn.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://knu.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://rvl.sweek.top

JS:   /\d+/.test(s)
来源：http://gwy.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://gqi.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jcu.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sdl.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://xcc.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yyg.tianlin.xyz

[I02] 提取所有匹配
来源：http://fvh.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://svs.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cyy.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://stj.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://ykh.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cnh.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://voo.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://tqj.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oog.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://rtx.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iiy.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cry.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ina.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ypd.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://peq.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cvj.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xhf.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nhp.yvedp.cn

[I04] 正则替换
来源：http://yoz.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://txq.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tpq.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://cay.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vtx.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://ihs.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ohb.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://flk.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gre.ydjk.org.cn

[I05] 按正则拆分
来源：http://utv.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xre.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://usp.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://xce.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://ykq.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://ghc.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qqv.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://tmb.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aiq.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://piz.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vgl.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://myp.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hbv.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjs.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fdi.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yge.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://usm.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vwn.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://gsk.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mcf.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yfm.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vnu.wangshuangyany.cn

TS:   /error/gim
来源：http://hhl.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rtf.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bpu.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://bwm.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iwt.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://ytn.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jqz.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hwx.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bhq.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://msz.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://viw.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://myn.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ptb.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nwu.gaohongyu789.top

================================================================================
来源：http://zoh.epnwcf.com

J. 日期与时间
来源：http://jwo.ydjk.org.cn

================================================================================
来源：http://yhm.jiagoushi.top

[J01] 获取当前时间
来源：http://znr.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://djz.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://npy.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://wun.nwbrower.top

TS:   new Date();  Date.now()
来源：http://exc.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jox.chenzaomai.com

Go:   time.Now()
来源：http://tpu.hcnkem.com

Ruby: Time.now
来源：http://xgz.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ifa.smart0.xyz

[J02] 格式化输出
来源：http://rsb.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ykl.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vja.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://isc.zhixingplan.top

TS:   d.toISOString()
来源：http://fvr.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://our.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wbt.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://and.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ied.jianghu66.top

[J03] 字符串解析为日期
来源：http://bin.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sca.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iry.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://ctt.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://nti.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://vqj.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kua.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://bwg.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jma.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://rrc.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qmv.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vap.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trr.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://wgv.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pkf.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://woo.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kfu.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hdm.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://ytz.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://yhn.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://utb.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gjx.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jfo.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://nfs.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ppl.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://hwg.aibaodan.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jzi.ybcxt.top

[J06] 计算两时间之差
来源：http://xoo.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://cvk.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://emt.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://teb.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dem.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://tou.sweek.top

Go:   end.Sub(start).Hours()
来源：http://wyy.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://qcp.sweek.top

C#:   (end - start).TotalSeconds
来源：http://att.zhijiandao.cn


<!-- 参考信息 -->