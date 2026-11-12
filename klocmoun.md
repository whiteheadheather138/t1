代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://nty.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://shk.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wwh.sweek.top

TS:   interface Shape { area(): number; }
来源：http://lot.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://ydm.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://jyc.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xbr.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://dao.shanyushiyangtech.top

[G10] 访问控制
来源：http://nmv.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://dug.vqdsnc.cn

PHP:  public / protected / private
来源：http://lzm.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://fdw.zycfv.cn

TS:   public / protected / private
来源：http://xvv.meibo888.top

Java: public / protected / private / 默认包级
来源：http://euo.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://bur.gotoacloud.top

Ruby: public / protected / private
来源：http://zrm.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://cca.yangfankeji.com

[G11] getter / setter
来源：http://wcn.tarul.cn

Py:   @property 与 @x.setter
来源：http://nsa.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xyj.ydzc1.top

JS:   get name() { return this._name; }
来源：http://ain.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://efm.yfazqb.com

Java: public String getName() { return name; }
来源：http://wtj.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lud.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://oxh.yueranfly.top

C#:   public string Name { get; set; }
来源：http://xld.bjfxy.top

[G12] 对象转字符串
来源：http://tqb.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://jje.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://igm.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://kya.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://fmh.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://byp.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://ckp.iojbl.cn

Ruby: def to_s; @name; end
来源：http://vjq.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://epj.sjlbkw.cn

[G13] 判断对象类型
来源：http://cfa.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://vda.yj20258888.top

PHP:  $u instanceof User
来源：http://adj.jqgfzy.top

JS:   u instanceof User
来源：http://yxf.guannengcc.top

TS:   u instanceof User
来源：http://kao.jqgfzy.top

Java: u instanceof User
来源：http://uvz.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ihb.aizwys.cn

Ruby: u.is_a?(User)
来源：http://yff.chenjidiqi.icu

C#:   u is User
来源：http://rcr.fengsongda.top

[G14] 数据类 / record
来源：http://wep.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tzk.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://ail.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oky.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://ytj.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://djy.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://wtq.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kln.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://ajv.9152youxi.cn

[G15] 枚举
来源：http://zle.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cdq.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jly.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xby.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rvx.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://xij.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rqc.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://fjm.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gyn.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://bsw.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mzj.cheryme.top

PHP:  get_object_vars($obj);
来源：http://ull.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://vkf.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://sfp.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uip.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dmw.sysykeji.top

Ruby: obj.instance_variables
来源：http://rbi.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://xag.jinyuanbaomall.cn

================================================================================
来源：http://dnn.bjfxy.top

H. 异常与错误处理
来源：http://tct.haohaochexian.top

================================================================================
来源：http://uzq.sjlbkw.cn

[H01] try / catch 基础
来源：http://nec.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fev.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jso.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tij.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wns.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ydy.ppjwa.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sbo.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fpc.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ruo.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://ufz.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://uip.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aqh.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://odf.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dez.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://syh.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wqf.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lsx.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://upr.cqqwz.cn

[H03] 主动抛出异常
来源：http://nlh.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://fku.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qdx.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://rat.hammf.cn

TS:   throw new Error("错误信息");
来源：http://ope.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tws.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mvp.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qni.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://fou.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://hxn.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://bho.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://cgn.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://xzg.hesvh.cn

TS:   class MyError extends Error {}
来源：http://kdo.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://vol.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ucs.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://nxu.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://mje.tianlin.xyz

[H05] 捕获特定类型
来源：http://wyx.gaohongyu789.top

Py:   except ValueError as e:
来源：http://scf.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://odo.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://gfi.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://ceo.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://jxl.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vvj.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://anh.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dze.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://xax.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://tyv.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://lrh.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jhu.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zjj.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hqr.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qkw.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://ezj.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://bqx.cheryme.top

[H07] 断言
来源：http://wkw.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://kqk.cucudq.cn

PHP:  assert($x > 0);
来源：http://byn.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://ayt.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://iju.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://qea.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ywd.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://plt.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://bxs.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://kye.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://qlt.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bsp.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://euh.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iks.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ejh.xinyue.icu

Go:   err.Error()
来源：http://iwb.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://kyi.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://mjn.316326.xyz

[H09] 带错误码的异常
来源：http://tvn.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yiu.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://jdp.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ygc.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xia.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hyq.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cfa.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aoh.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ble.feifeiyinyue.top

[H10] 资源自动释放
来源：http://dfq.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://foy.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mvb.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iuy.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iqp.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ztm.fengsongda.top

Go:   defer f.Close()
来源：http://ebx.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://alj.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://obs.gogol.net.cn

================================================================================
来源：http://ugt.ppjwa.cn

I. 正则表达式
来源：http://lam.316326.xyz

================================================================================
来源：http://rdc.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://ibj.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://une.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://qva.mhx1999.top

JS:   /\d+/.test(s)
来源：http://kmi.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://jym.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uuf.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tkl.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://jad.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jnv.cashguo.top

[I02] 提取所有匹配
来源：http://fsz.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://jmj.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xwt.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://doo.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://qsw.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xgg.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zmw.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://jqx.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ild.smart0.xyz

[I03] 提取捕获分组
来源：http://fql.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lry.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hqg.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rno.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rud.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bvq.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://epl.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hnj.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dti.fengsongda.top

[I04] 正则替换
来源：http://lge.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lxb.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xhe.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yaf.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xju.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://uni.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yxl.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zop.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xdf.52xcode.cn

[I05] 按正则拆分
来源：http://hbk.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oak.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dot.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://dal.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://tvb.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://uml.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ahj.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://flz.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lkz.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wld.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pdg.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xoo.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ydq.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ssh.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tnc.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tmn.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bwl.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qbv.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://jiy.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jnt.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qkl.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hmt.c1oappe.top

TS:   /error/gim
来源：http://nct.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zqh.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tmk.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://kts.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hec.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://dkc.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pkr.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gfc.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://foj.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://afh.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ebi.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jdr.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fnj.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hmm.ydzc1.top

================================================================================
来源：http://pgf.zdqjudy.top

J. 日期与时间
来源：http://jvn.yj20258.top

================================================================================
来源：http://raf.cucudq.cn

[J01] 获取当前时间
来源：http://gbo.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ykb.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eiu.sxryk.cn

JS:   new Date();  Date.now()
来源：http://tfx.yonumen.top

TS:   new Date();  Date.now()
来源：http://wxv.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cax.wangdashe.top

Go:   time.Now()
来源：http://tkv.ehwqpu.com

Ruby: Time.now
来源：http://pri.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jdk.bjfxy.top

[J02] 格式化输出
来源：http://lvn.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jrs.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vik.ivvv.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ldh.zdqjudy.top

TS:   d.toISOString()
来源：http://zxb.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eyt.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wvl.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uxg.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://suf.chenzaomai.com

[J03] 字符串解析为日期
来源：http://ulh.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yup.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ocw.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://kxf.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://lsf.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://qqp.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lno.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://cec.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zml.tian-w.cn

[J04] 时间戳与日期互转
来源：http://gxg.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ayd.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ash.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lku.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://edp.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rkf.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://snw.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aet.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://idm.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://xda.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://hgx.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zjw.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hxj.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://adn.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://zde.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tqx.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://dht.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://voy.xuanzx.com

[J06] 计算两时间之差
来源：http://ypz.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://ltd.xziqi.cn

PHP:  $end->diff($start)->days;
来源：http://xrw.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iey.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lew.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://kit.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://ghe.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://oca.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://upq.jqgufenzy.top

[J07] 比较两个日期
来源：http://bmv.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://iqu.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ihc.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ifm.bjfxy.top


<!-- 参考信息 -->