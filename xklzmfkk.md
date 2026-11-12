代发 wailian999

Java: interface Shape { double area(); }
来源：http://cfq.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://hfk.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zuv.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://yeu.yongpay.top

[G10] 访问控制
来源：http://jvj.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://bkl.vqdsnc.cn

PHP:  public / protected / private
来源：http://pbu.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://jrb.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://bfj.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://dum.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dcz.chenlongwang.top

Ruby: public / protected / private
来源：http://rkp.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://xyb.fktsv.cn

[G11] getter / setter
来源：http://hbk.jqgufenzy.top

Py:   @property 与 @x.setter
来源：http://jmj.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://dua.vehdjk.com

JS:   get name() { return this._name; }
来源：http://zrc.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://fow.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://mxh.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ori.hnxiangtu.top

Ruby: attr_accessor :name
来源：http://cgb.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://jod.zycfv.cn

[G12] 对象转字符串
来源：http://jmw.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://nic.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mge.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://aam.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://zri.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://ecl.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://orr.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://lyx.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://cqq.jyoumei.cn

[G13] 判断对象类型
来源：http://jmu.cucudq.cn

Py:   isinstance(u, User)
来源：http://cfv.tarul.cn

PHP:  $u instanceof User
来源：http://fmb.yangfankeji.com

JS:   u instanceof User
来源：http://mdr.sweek.top

TS:   u instanceof User
来源：http://nkq.fengsongda.top

Java: u instanceof User
来源：http://kyz.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://vuq.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://ocj.sysykeji.top

C#:   u is User
来源：http://vph.andypj.xyz

[G14] 数据类 / record
来源：http://sde.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zxl.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://ozh.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://osh.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://bwc.xziqi.cn

Java: record User(String name, int age) {}
来源：http://red.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://xdu.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lrc.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://zui.cashguo.top

[G15] 枚举
来源：http://rht.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nan.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mif.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://btz.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hlr.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://qbr.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tpq.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://xrf.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gre.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://eyr.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cmi.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://gvr.xuanzx.com

JS:   Object.entries(obj)
来源：http://frp.jqgfzy.top

TS:   Object.entries(obj)
来源：http://zny.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fml.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ydb.yj20258.top

Ruby: obj.instance_variables
来源：http://gqb.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://uec.wangshuangyany.cn

================================================================================
来源：http://auu.ydjk.org.cn

H. 异常与错误处理
来源：http://hbv.gaohongyu789.top

================================================================================
来源：http://arp.yongpay.top

[H01] try / catch 基础
来源：http://nvu.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://syw.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://znj.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cuj.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://awb.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cdm.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://anx.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qlx.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gbz.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://elc.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://tew.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yyt.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oke.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://pwg.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zyh.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gua.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fbx.bbcook.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://shj.redwolf501.top

[H03] 主动抛出异常
来源：http://ocd.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://lrk.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jfx.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://trr.fzhhl.top

TS:   throw new Error("错误信息");
来源：http://ovu.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://rej.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dxw.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hwv.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ukl.sjlbkw.cn

[H04] 自定义异常类型
来源：http://ihc.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://ete.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://shp.ivvv.top

JS:   class MyError extends Error {}
来源：http://xma.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://pay.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://lud.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ctt.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://xwg.bbcook.cn

C#:   class MyException : Exception {}
来源：http://exj.yj20258888.top

[H05] 捕获特定类型
来源：http://die.dashuyun.cn

Py:   except ValueError as e:
来源：http://kvu.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cba.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://fyk.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://yvf.jianghu66.top

Java: catch (IOException | SQLException e) {}
来源：http://pdu.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://etv.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://elk.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ras.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://wwz.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://yew.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kdh.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lwg.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gnr.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zsu.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ory.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://vgm.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://ubw.xylfe.cn

[H07] 断言
来源：http://owc.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://inr.snrcjt.cn

PHP:  assert($x > 0);
来源：http://gsp.cucudq.cn

JS:   console.assert(x > 0);
来源：http://sul.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://ncc.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://sud.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fdj.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nmy.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://fwx.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://mev.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://klm.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qla.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://nwo.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ahh.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gxp.gzhubu.top

Go:   err.Error()
来源：http://sbk.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://ulj.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://yel.cqqwz.cn

[H09] 带错误码的异常
来源：http://obr.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ofa.haohaochexian.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uci.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://asr.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zlh.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://glb.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mid.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://jxb.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rkk.snrcjt.cn

[H10] 资源自动释放
来源：http://npe.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lrj.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zvb.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cup.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://okq.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://crn.jianghu66.top

Go:   defer f.Close()
来源：http://ckx.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xec.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nqp.gaohongyu789.top

================================================================================
来源：http://itp.havefunace.top

I. 正则表达式
来源：http://qcq.c1oappe.top

================================================================================
来源：http://jqg.chenzaomai.com

[I01] 判断是否匹配
来源：http://jtx.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fmh.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://ied.meibo888.top

JS:   /\d+/.test(s)
来源：http://osp.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://kqa.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pgo.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wmo.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://qhg.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://efd.hammf.cn

[I02] 提取所有匹配
来源：http://cgg.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://yjh.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bqa.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mmq.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://cvi.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ffc.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ufu.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://sur.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://czv.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://cxv.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tft.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://erp.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oke.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wbj.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ich.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pwr.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mob.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ejx.sxryk.cn

[I04] 正则替换
来源：http://etz.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mut.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zcd.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://lug.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://cwq.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://brb.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jcc.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zcz.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xmm.sweek.top

[I05] 按正则拆分
来源：http://rcb.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nwv.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bvg.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://iln.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://hjs.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://vcp.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qlm.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bmv.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hta.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://myj.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jsf.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vwq.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdq.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vsi.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rrg.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ucf.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hue.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://azo.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://qnc.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nzt.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nkp.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nxt.yuanzhike.top

TS:   /error/gim
来源：http://xtt.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://age.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jib.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://yql.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bqm.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://ipv.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://flp.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jiy.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rus.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kbe.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lkd.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dix.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rbq.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jmv.iojbl.cn

================================================================================
来源：http://iul.52xcode.cn

J. 日期与时间
来源：http://pof.ydjk.org.cn

================================================================================
来源：http://mgf.guannengcc.top

[J01] 获取当前时间
来源：http://gzq.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://fdp.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nah.fehbvm.com

JS:   new Date();  Date.now()
来源：http://upy.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://lhc.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://obn.havefunace.top

Go:   time.Now()
来源：http://hrk.hongshengwenyu.top

Ruby: Time.now
来源：http://gzf.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lef.andypj.xyz

[J02] 格式化输出
来源：http://jsq.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iej.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cgx.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dgm.yongpay.top

TS:   d.toISOString()
来源：http://qvy.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lov.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://omv.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ywj.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zzo.hfpthk.cn

[J03] 字符串解析为日期
来源：http://cdv.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oll.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://shf.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://opl.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://lzc.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jpc.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://obk.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://nct.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zie.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://coh.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cpo.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kuu.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pma.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vbj.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ofl.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vpk.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wjv.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zgn.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://rtw.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://esk.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cnw.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcp.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rwz.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://pmh.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pkm.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://bkb.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://nez.gzhubu.top

[J06] 计算两时间之差
来源：http://oxw.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://mrw.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://wch.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sbp.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mwh.bbcook.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lmu.sweek.top

Go:   end.Sub(start).Hours()
来源：http://bsq.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://jqj.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://zbf.wangshuangyany.cn

[J07] 比较两个日期
来源：http://diu.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://fxe.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://huz.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://flf.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://wpi.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hfw.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://obd.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://drs.xuanzx.com


<!-- 参考信息 -->