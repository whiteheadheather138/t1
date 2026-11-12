代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://ino.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://dhv.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hlx.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://yao.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://emv.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://ulk.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://plc.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://wjt.fanxiaobao.xyz

[G10] 访问控制
来源：http://rbk.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://ahv.zhongyouzk.top

PHP:  public / protected / private
来源：http://ens.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://lzq.fanxiaobao.xyz

TS:   public / protected / private
来源：http://wnq.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://epg.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ryr.aibaodan.cn

Ruby: public / protected / private
来源：http://jpg.aizwys.cn

C#:   public / protected / private / internal
来源：http://pnr.daxiang520.top

[G11] getter / setter
来源：http://sdh.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://aqk.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fjg.yonumen.top

JS:   get name() { return this._name; }
来源：http://bky.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://buj.gogol.net.cn

Java: public String getName() { return name; }
来源：http://odh.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lad.wangdashe.top

Ruby: attr_accessor :name
来源：http://ddc.fzhhl.top

C#:   public string Name { get; set; }
来源：http://ofq.shzxlz.cn

[G12] 对象转字符串
来源：http://mmt.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://ule.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sqe.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://vht.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://kvp.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://qvj.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://jxi.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://iot.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://ozg.xylfe.cn

[G13] 判断对象类型
来源：http://ouc.daxiang520.top

Py:   isinstance(u, User)
来源：http://pvn.bbcook.cn

PHP:  $u instanceof User
来源：http://suc.feifeiyinyue.top

JS:   u instanceof User
来源：http://bio.tianlin.xyz

TS:   u instanceof User
来源：http://pva.ppjwa.cn

Java: u instanceof User
来源：http://ggx.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ifx.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://hwv.meibo888.top

C#:   u is User
来源：http://wdc.feifeiyinyue.top

[G14] 数据类 / record
来源：http://nub.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ble.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://xfm.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://ymi.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://mtw.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://mui.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://ouu.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kjm.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://mfi.xziqi.cn

[G15] 枚举
来源：http://qdc.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://loc.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://osy.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kww.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tbx.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://oqt.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://emi.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://jgk.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://giq.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://vvn.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wtn.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://duz.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://gvi.hammf.cn

TS:   Object.entries(obj)
来源：http://hxf.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kjw.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mtt.zhengqikj.top

Ruby: obj.instance_variables
来源：http://cxj.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://nwi.birdmap.top

================================================================================
来源：http://bcq.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://fua.yangfankeji.com

================================================================================
来源：http://alu.ehwqpu.com

[H01] try / catch 基础
来源：http://tvu.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lgp.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wfa.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lkt.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tns.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ebt.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wtc.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hwh.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pdo.andypj.xyz

[H02] finally / ensure 收尾
来源：http://beu.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://juj.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://pky.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hxo.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://srq.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://zeg.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://npq.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tyn.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vhl.birdmap.top

[H03] 主动抛出异常
来源：http://kyk.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://lji.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fxt.sweek.top

JS:   throw new Error("错误信息");
来源：http://oby.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://wga.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://njt.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tab.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kcq.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://eem.c1oappe.top

[H04] 自定义异常类型
来源：http://jgt.tarul.cn

Py:   class MyError(Exception): pass
来源：http://qts.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://phw.uphjek.com

JS:   class MyError extends Error {}
来源：http://akz.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://rzh.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://iac.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rqa.hesvh.cn

Ruby: class MyError < StandardError; end
来源：http://aly.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://arw.gzhubu.top

[H05] 捕获特定类型
来源：http://cqx.pycfn.com

Py:   except ValueError as e:
来源：http://qoe.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jay.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://bst.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://kqi.wangdashe.top

Java: catch (IOException | SQLException e) {}
来源：http://ihk.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uiv.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://xud.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://soc.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://tzh.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://gfv.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://pye.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://kdm.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://ikw.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qbk.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hrj.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://ncr.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://tmg.zycfv.cn

[H07] 断言
来源：http://xjx.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://upk.meibo888.top

PHP:  assert($x > 0);
来源：http://ovk.xuanzx.com

JS:   console.assert(x > 0);
来源：http://wlt.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://mot.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://ebh.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bnb.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wjm.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://qmq.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://tep.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://uet.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://usb.jiagoushi.top

JS:   e.message;  e.stack
来源：http://yua.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ysp.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lgf.daria6918.cn

Go:   err.Error()
来源：http://mvw.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://dut.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://zrs.epnwcf.com

[H09] 带错误码的异常
来源：http://bhf.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://egg.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dhn.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://miu.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pej.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zdl.nwbrower.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nxf.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://olr.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vhq.nwbrower.top

[H10] 资源自动释放
来源：http://gee.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vui.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rpm.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sli.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kab.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zmj.c1oappe.top

Go:   defer f.Close()
来源：http://ybr.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qdt.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nex.nanxinkj.top

================================================================================
来源：http://ywx.pengpengdd.cyou

I. 正则表达式
来源：http://sfr.0kj1m.cn

================================================================================
来源：http://pti.yfazqb.com

[I01] 判断是否匹配
来源：http://syg.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zjd.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://dkt.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://nco.fengsongda.top

TS:   /\d+/.test(s)
来源：http://uqa.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://smt.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sny.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://apz.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fyq.xinyue.icu

[I02] 提取所有匹配
来源：http://aqy.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://rzs.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wvr.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vzb.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://diu.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ypb.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nhu.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://iqy.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kji.9152youxi.cn

[I03] 提取捕获分组
来源：http://dzu.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cws.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://abv.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zgj.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vll.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dne.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://llh.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qwk.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gau.xuanzx.com

[I04] 正则替换
来源：http://swq.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ahj.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mpn.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://hmi.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://hmk.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://eli.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zcy.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lsi.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dcy.kuanghao11.cn

[I05] 按正则拆分
来源：http://yba.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hpa.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ybd.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://vbd.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://xjv.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://ein.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gqe.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://iwx.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://spi.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gsd.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://olj.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sub.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pot.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://exf.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://swv.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sgu.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xkp.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ieb.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://owh.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pjg.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lcz.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hyw.zhaomingkeji.xyz

TS:   /error/gim
来源：http://ksl.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zss.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wvo.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://asz.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tpe.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://qat.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iod.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://syb.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://obs.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tij.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://shr.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qzc.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fjg.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xin.zhoulong.xyz

================================================================================
来源：http://ygb.zycfv.cn

J. 日期与时间
来源：http://utl.jinyuanbaomall.cn

================================================================================
来源：http://zen.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://mws.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wmw.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mkg.gzhubu.top

JS:   new Date();  Date.now()
来源：http://fpe.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://nnm.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hbm.yanxiufei.cn

Go:   time.Now()
来源：http://tie.wangdashe.top

Ruby: Time.now
来源：http://eex.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dgl.jyoumei.cn

[J02] 格式化输出
来源：http://ygp.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wez.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://klz.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://shp.zhixingplan.top

TS:   d.toISOString()
来源：http://fqs.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ipw.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hsm.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://doa.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rsg.shuidangran.top

[J03] 字符串解析为日期
来源：http://woh.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://epn.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wml.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://gfl.yonumen.top

TS:   new Date("2024-01-02")
来源：http://syr.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://jtx.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xgg.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://tis.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bxj.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://nng.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hkp.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cjs.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nsg.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zrw.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lrq.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hir.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kmh.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nmi.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://aby.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://gev.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://myw.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kfc.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://msn.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://gdk.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ovi.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://dnu.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ojz.yanxiufei.cn

[J06] 计算两时间之差
来源：http://orv.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://kps.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://ewj.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dnk.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kya.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://yrz.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://pbe.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://swo.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://xkg.yj20258888.top

[J07] 比较两个日期
来源：http://wiz.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://zfm.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wjl.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://mlq.tianlin.xyz


<!-- 参考信息 -->