代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://mxf.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://vnw.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pvi.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://hor.yj20258888.top

Java: interface Shape { double area(); }
来源：http://uxs.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://nfh.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://upj.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://gxt.c1oappe.top

[G10] 访问控制
来源：http://wfd.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://eod.gzhubu.top

PHP:  public / protected / private
来源：http://snq.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://dju.jinghuilouyu.cn

TS:   public / protected / private
来源：http://gna.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://aja.nanxinkj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nns.jqgfzy.top

Ruby: public / protected / private
来源：http://wff.svipenyu.cn

C#:   public / protected / private / internal
来源：http://jyu.tian-w.cn

[G11] getter / setter
来源：http://lyu.tanke756.top

Py:   @property 与 @x.setter
来源：http://ltd.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rfl.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://ahb.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://fgt.ctjpmb.com

Java: public String getName() { return name; }
来源：http://xiy.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://nry.zhengqikj.top

Ruby: attr_accessor :name
来源：http://pvb.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://mxi.yj20258888.top

[G12] 对象转字符串
来源：http://sni.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://vif.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zpz.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://yhk.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://yzn.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://fgr.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://gvl.yvedp.cn

Ruby: def to_s; @name; end
来源：http://etv.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://hid.yvedp.cn

[G13] 判断对象类型
来源：http://ayt.9152youxi.cn

Py:   isinstance(u, User)
来源：http://uby.epnwcf.com

PHP:  $u instanceof User
来源：http://cbe.sysykeji.top

JS:   u instanceof User
来源：http://xzx.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://ngf.feifeiyinyue.top

Java: u instanceof User
来源：http://zbd.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hoo.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://vvc.mhx1999.top

C#:   u is User
来源：http://aro.yueranfly.top

[G14] 数据类 / record
来源：http://yvs.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://djk.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://dqq.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://cxs.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://cds.daxiang520.top

Java: record User(String name, int age) {}
来源：http://gxu.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://voo.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ulk.yonumen.top

C#:   record User(string Name, int Age);
来源：http://wyc.redwolf501.top

[G15] 枚举
来源：http://utr.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dqc.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cph.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mfd.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kkr.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://zeq.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bxx.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://say.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kxn.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://gcs.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hoa.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://nrg.zhixingplan.top

JS:   Object.entries(obj)
来源：http://ngj.uphjek.com

TS:   Object.entries(obj)
来源：http://gra.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ukf.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://amn.daria6918.cn

Ruby: obj.instance_variables
来源：http://vnt.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://vtn.c1oappe.top

================================================================================
来源：http://fts.xuanzx.com

H. 异常与错误处理
来源：http://gyq.smart0.xyz

================================================================================
来源：http://fvf.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://hqm.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ihd.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qcy.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://acp.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lpf.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eqj.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://idz.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pvi.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nbg.cheryme.top

[H02] finally / ensure 收尾
来源：http://htn.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://yii.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://liz.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://xuu.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ybp.nanxuanxn.top

Java: try { f(); } finally { cleanup(); }
来源：http://jyv.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wpl.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qxl.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://caz.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://epc.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://csy.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pzq.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://qns.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://apf.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://umk.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ucs.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uub.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jzg.epnwcf.com

[H04] 自定义异常类型
来源：http://ajv.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://edv.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://ifo.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://awc.hesvh.cn

TS:   class MyError extends Error {}
来源：http://xlk.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://txf.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://brz.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://yea.cashguo.top

C#:   class MyException : Exception {}
来源：http://dce.guowangkeji.top

[H05] 捕获特定类型
来源：http://nsv.yvedp.cn

Py:   except ValueError as e:
来源：http://poa.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tdh.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://geb.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://nyp.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://yhb.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jsy.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://yrl.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uyw.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://wwz.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://pio.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://tgj.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://acg.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://lgo.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yme.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://muh.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://ltv.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://trd.nanxinkj.top

[H07] 断言
来源：http://xab.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://hjw.52xcode.cn

PHP:  assert($x > 0);
来源：http://nfy.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://kqx.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://vry.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://pjv.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bfx.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://mmr.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://tou.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://fwb.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://xfp.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fcu.bbcook.cn

JS:   e.message;  e.stack
来源：http://ilb.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ldd.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dlz.yangfankeji.com

Go:   err.Error()
来源：http://rrk.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://xkt.tianlin.xyz

C#:   e.Message;  e.StackTrace
来源：http://rxq.dianchejie.cn

[H09] 带错误码的异常
来源：http://kpv.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wmx.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xro.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dwu.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kem.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kke.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://crv.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://cju.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ytr.tian-w.cn

[H10] 资源自动释放
来源：http://pxq.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vph.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kxl.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://muu.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rkm.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://spv.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://blv.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://knn.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nor.yj20258888.top

================================================================================
来源：http://kkt.cheryme.top

I. 正则表达式
来源：http://hpp.c1oappe.top

================================================================================
来源：http://pvh.cucudq.cn

[I01] 判断是否匹配
来源：http://yah.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dxm.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://suz.cheryme.top

JS:   /\d+/.test(s)
来源：http://mzy.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://zpn.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ljs.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jzi.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://yym.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mbg.aizwys.cn

[I02] 提取所有匹配
来源：http://uke.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://gci.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qtd.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nlw.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://ylv.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://waz.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://prm.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://ucc.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jcf.gzhubu.top

[I03] 提取捕获分组
来源：http://zey.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ynt.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dlp.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://anz.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uuu.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hli.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jpu.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wtf.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zse.tian-w.cn

[I04] 正则替换
来源：http://hlh.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zsy.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmi.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://dbd.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ccz.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://sxp.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zxl.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://igs.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yph.yangfankeji.com

[I05] 按正则拆分
来源：http://jst.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://yyu.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xte.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://pse.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://gzr.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://ygf.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ajq.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://top.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kvg.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jpd.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hge.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://efm.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bre.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lrv.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ebe.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pyd.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gxh.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zut.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://pdj.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lce.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tkf.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://snv.dianchejie.cn

TS:   /error/gim
来源：http://juo.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://myd.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://htn.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://fli.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tec.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://weh.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imi.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wve.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pbf.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qfc.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://pfx.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zls.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ycg.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jge.svipenyu.cn

================================================================================
来源：http://tcp.xylfe.cn

J. 日期与时间
来源：http://ejz.xziqi.cn

================================================================================
来源：http://blz.pycfn.com

[J01] 获取当前时间
来源：http://xpj.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aoy.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qxj.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://mbp.mhx1999.top

TS:   new Date();  Date.now()
来源：http://fie.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eoi.redwolf501.top

Go:   time.Now()
来源：http://vkt.jiagoushi.top

Ruby: Time.now
来源：http://ufa.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uka.ydzc1.top

[J02] 格式化输出
来源：http://urv.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqi.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zye.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://buy.tanke756.top

TS:   d.toISOString()
来源：http://eqc.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fna.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bvk.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oik.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hox.bbcook.cn

[J03] 字符串解析为日期
来源：http://tdo.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vun.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mhl.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://emw.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://ley.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dac.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vjr.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://mjp.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gso.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://fez.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://opt.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fxb.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dne.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ohp.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bwr.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cnz.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qkp.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bay.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://vfq.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://qrl.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://iuh.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uky.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aps.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://ngp.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jos.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://skw.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://abx.guannengcc.top

[J06] 计算两时间之差
来源：http://puc.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://lol.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://hmw.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dol.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uja.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://biv.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://omd.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://igm.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://juw.dashuyun.cn

[J07] 比较两个日期
来源：http://fvl.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://rlh.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mai.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jke.yueranfly.top


<!-- 参考信息 -->