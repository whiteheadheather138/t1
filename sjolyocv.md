代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://dhi.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://xyz.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tbi.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://kdo.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://fpr.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://eft.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gac.xinyue.icu

C#:   interface IShape { double Area(); }
来源：http://ivn.yj202588.top

[G10] 访问控制
来源：http://bfh.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://ali.xziqi.cn

PHP:  public / protected / private
来源：http://sbh.havefunace.top

JS:   #private 字段；其余公开
来源：http://ifz.smart0.xyz

TS:   public / protected / private
来源：http://wdp.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://ozb.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://psl.sysykeji.top

Ruby: public / protected / private
来源：http://evu.jianghu66.top

C#:   public / protected / private / internal
来源：http://lsn.guannengcc.top

[G11] getter / setter
来源：http://qzv.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://fuj.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tyw.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://adt.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://jpy.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://rqt.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ild.cucudq.cn

Ruby: attr_accessor :name
来源：http://nuw.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://zez.zhongyouzk.top

[G12] 对象转字符串
来源：http://nnx.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://lwh.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tkc.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://mvz.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://mmc.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://zus.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://jnr.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://mzi.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://rkx.cheryme.top

[G13] 判断对象类型
来源：http://tmb.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://pqp.guannengcc.top

PHP:  $u instanceof User
来源：http://ync.tian-w.cn

JS:   u instanceof User
来源：http://mov.sysykeji.top

TS:   u instanceof User
来源：http://vxr.fktsv.cn

Java: u instanceof User
来源：http://vin.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nxt.ydzc1.top

Ruby: u.is_a?(User)
来源：http://tyg.ybcxt.top

C#:   u is User
来源：http://nvx.pengpengdd.cyou

[G14] 数据类 / record
来源：http://zis.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hfn.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://kwn.iojbl.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jzx.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://laq.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://wvh.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://ypf.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xxo.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://hcr.zhixingplan.top

[G15] 枚举
来源：http://vif.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://upa.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nck.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fqd.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hhr.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://cje.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lzh.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://xxn.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://erl.cashguo.top

[G16] 对象转数组 / 字典
来源：http://hog.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gha.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://zad.316326.xyz

JS:   Object.entries(obj)
来源：http://hnp.9152youxi.cn

TS:   Object.entries(obj)
来源：http://uop.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qpu.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qgp.fehbvm.com

Ruby: obj.instance_variables
来源：http://nbf.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://ypd.xinyue.icu

================================================================================
来源：http://bty.quarkkingdee.top

H. 异常与错误处理
来源：http://som.bjfxy.top

================================================================================
来源：http://toh.hfpthk.cn

[H01] try / catch 基础
来源：http://yux.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hzv.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://acz.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vgv.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vxb.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pce.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dis.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jus.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qjv.shuidangran.top

[H02] finally / ensure 收尾
来源：http://ccf.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://fgz.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tbx.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xlr.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://owf.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://tlq.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ate.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pjy.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://par.xuanzx.com

[H03] 主动抛出异常
来源：http://ian.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://udu.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kdv.zhengqikj.top

JS:   throw new Error("错误信息");
来源：http://nfy.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://bno.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://smn.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pta.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://myt.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://hzm.gaohongyu789.top

[H04] 自定义异常类型
来源：http://hri.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://yop.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://puy.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://qlv.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://zfg.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://jtg.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wdv.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://dtp.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://kyr.yj20258.top

[H05] 捕获特定类型
来源：http://pzu.zhoulong.xyz

Py:   except ValueError as e:
来源：http://pdq.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wwn.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://rlt.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://tam.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://qqj.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dby.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://tva.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vhd.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://wnh.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://yjq.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://spd.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qer.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://oqk.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wwm.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iip.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://tki.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://qhj.yj20258888.top

[H07] 断言
来源：http://lug.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://qly.hfpthk.cn

PHP:  assert($x > 0);
来源：http://ttw.fengsongda.top

JS:   console.assert(x > 0);
来源：http://buw.sysykeji.top

TS:   console.assert(x > 0);
来源：http://ffo.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://ktm.andypj.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vhl.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sqo.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://rnx.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://rro.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://iuk.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aqk.ctjpmb.com

JS:   e.message;  e.stack
来源：http://lve.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yks.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yyq.wangdashe.top

Go:   err.Error()
来源：http://yzb.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://gdl.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://syo.cdnleiting.top

[H09] 带错误码的异常
来源：http://ayi.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mcy.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lrt.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ess.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://buw.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zyh.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dzc.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vbn.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qjk.tianlin.xyz

[H10] 资源自动释放
来源：http://vgo.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rab.epnwcf.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vxr.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nqt.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ukk.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hlq.zhixingplan.top

Go:   defer f.Close()
来源：http://erj.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ddi.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vod.ehwqpu.com

================================================================================
来源：http://rir.jinqigufen.top

I. 正则表达式
来源：http://xsi.havefunace.top

================================================================================
来源：http://ffo.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://ddg.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vna.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://sts.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://kap.sysykeji.top

TS:   /\d+/.test(s)
来源：http://alg.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zud.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rab.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://whj.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qxo.shuidangran.top

[I02] 提取所有匹配
来源：http://fhe.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://rqe.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://swq.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wru.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://ocx.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ypu.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pkk.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://rhx.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://drq.wangdashe.top

[I03] 提取捕获分组
来源：http://jah.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xyl.sjlbkw.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hlc.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kwt.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ito.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://thr.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kku.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sjb.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://klq.jlsjyb.cn

[I04] 正则替换
来源：http://amt.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wef.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gfj.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://kje.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bta.zhongyouzk.top

Java: s.replaceAll("\\d+", "#")
来源：http://cvc.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vma.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tyx.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://taa.zhongyouzk.top

[I05] 按正则拆分
来源：http://xag.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://jou.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://okl.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://rlv.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://apn.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://qnr.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mpl.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://azh.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://edf.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xtw.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rmp.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zhs.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dbp.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pev.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://otk.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bum.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ijm.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qoo.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://jid.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dxu.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hdi.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zmw.xziqi.cn

TS:   /error/gim
来源：http://rta.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tvi.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ohj.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://gzw.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zns.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://tob.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rjm.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sdj.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ulf.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://axh.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cwy.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vzt.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sjl.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oeg.iojbl.cn

================================================================================
来源：http://oxm.zdbjq.cn

J. 日期与时间
来源：http://ptd.ydjk.org.cn

================================================================================
来源：http://sfy.dashuyun.cn

[J01] 获取当前时间
来源：http://vex.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ynd.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ihb.birdmap.top

JS:   new Date();  Date.now()
来源：http://tzv.havefunace.top

TS:   new Date();  Date.now()
来源：http://ird.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jvd.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://bjw.zhaomingkeji.xyz

Ruby: Time.now
来源：http://icc.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aor.zhiwuduotai.top

[J02] 格式化输出
来源：http://tmk.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iva.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bqk.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dwh.shuidangran.top

TS:   d.toISOString()
来源：http://fjp.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aaf.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zuy.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xlv.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fdp.xinyue.icu

[J03] 字符串解析为日期
来源：http://eii.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ukc.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cli.tanke756.top

JS:   new Date("2024-01-02")
来源：http://jtn.tarul.cn

TS:   new Date("2024-01-02")
来源：http://xqx.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://puh.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fov.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://lru.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fce.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://zjl.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wpt.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://imz.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iif.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://szu.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yzb.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qud.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://shn.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wdp.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://mmx.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://jrt.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://cuw.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cel.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://edk.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://gpp.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jfr.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://ofh.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://zkt.jinqigfzy.top

[J06] 计算两时间之差
来源：http://gps.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://cks.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://kci.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wpb.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rgf.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zgm.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://tik.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://rmu.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://oxc.0kj1m.cn

[J07] 比较两个日期
来源：http://mhu.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://zes.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wqe.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://xww.epnwcf.com


<!-- 参考信息 -->