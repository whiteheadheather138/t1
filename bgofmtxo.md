代发 wailian999

Java: interface Shape { double area(); }
来源：http://cqg.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://kja.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ljx.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://hws.zhaomingkeji.xyz

[G10] 访问控制
来源：http://lvv.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://dfn.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://bjk.fehbvm.com

JS:   #private 字段；其余公开
来源：http://fli.daria6918.cn

TS:   public / protected / private
来源：http://wlp.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://wki.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://aqm.zhengqikj.top

Ruby: public / protected / private
来源：http://smm.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://gdr.ybcxt.top

[G11] getter / setter
来源：http://cxu.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://geg.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sdq.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://erg.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://mtr.sufxvd.cn

Java: public String getName() { return name; }
来源：http://fsw.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kyk.hcnkem.com

Ruby: attr_accessor :name
来源：http://mkf.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://sif.daria6918.cn

[G12] 对象转字符串
来源：http://tgo.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://tji.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lld.tarul.cn

JS:   toString() { return this.name; }
来源：http://pzf.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://quv.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://tsy.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nxh.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://mdx.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://yfm.cheryme.top

[G13] 判断对象类型
来源：http://ekz.snrcjt.cn

Py:   isinstance(u, User)
来源：http://qeh.zhongyouzk.top

PHP:  $u instanceof User
来源：http://tyv.jqgfzy.top

JS:   u instanceof User
来源：http://jtu.cqqwz.cn

TS:   u instanceof User
来源：http://bql.yonumen.top

Java: u instanceof User
来源：http://vgp.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xhr.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://nwt.smart0.xyz

C#:   u is User
来源：http://xpz.9152youxi.cn

[G14] 数据类 / record
来源：http://ztn.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xjd.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://kig.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://tzd.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://cze.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://azf.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://stn.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://opp.tanke756.top

C#:   record User(string Name, int Age);
来源：http://iaw.chenlongwang.top

[G15] 枚举
来源：http://zao.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uij.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uoo.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rmz.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ukr.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://yfh.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oyr.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://yfb.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jbc.sweek.top

[G16] 对象转数组 / 字典
来源：http://rhb.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rom.tanke756.top

PHP:  get_object_vars($obj);
来源：http://cwx.daxiang520.top

JS:   Object.entries(obj)
来源：http://gxo.wangdashe.top

TS:   Object.entries(obj)
来源：http://bjg.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cpw.zdqjudy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://aue.aizwys.cn

Ruby: obj.instance_variables
来源：http://lss.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://kyy.hysaishi.cn

================================================================================
来源：http://qqm.fktsv.cn

H. 异常与错误处理
来源：http://tbj.yueranfly.top

================================================================================
来源：http://qnx.fehbvm.com

[H01] try / catch 基础
来源：http://fsn.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nqb.aizwys.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jui.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://paf.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xdr.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rtj.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://shj.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ote.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tug.hammf.cn

[H02] finally / ensure 收尾
来源：http://bai.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://tvn.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wdk.chenjidiqi.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://jrg.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kxf.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pbg.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://lgp.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xev.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cbk.yvedp.cn

[H03] 主动抛出异常
来源：http://ctd.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://zxu.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kwg.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://ogz.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://wll.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mkq.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://all.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://drd.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://nyx.xziqi.cn

[H04] 自定义异常类型
来源：http://pzl.cheryme.top

Py:   class MyError(Exception): pass
来源：http://vey.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://zuk.daria6918.cn

JS:   class MyError extends Error {}
来源：http://atq.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://ebj.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://lck.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://foj.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://yxz.yj202588.top

C#:   class MyException : Exception {}
来源：http://cao.uphjek.com

[H05] 捕获特定类型
来源：http://bdm.iojbl.cn

Py:   except ValueError as e:
来源：http://txv.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ubh.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://knt.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://xtg.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://hkz.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yle.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://yug.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://svo.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://kry.fktsv.cn

Py:   value = d.get("k") or default
来源：http://lbt.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://soa.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://azq.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://efn.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tid.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://axx.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://eik.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://hgl.zhaomingkeji.xyz

[H07] 断言
来源：http://utt.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://xga.tian-w.cn

PHP:  assert($x > 0);
来源：http://ccw.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://vma.hammf.cn

TS:   console.assert(x > 0);
来源：http://jdc.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://cpq.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wav.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://dfa.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://rmn.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://hrz.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ese.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bka.hfpthk.cn

JS:   e.message;  e.stack
来源：http://yib.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eox.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://enu.shanyushiyangkeji.top

Go:   err.Error()
来源：http://efj.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://owk.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://ymx.gogol.net.cn

[H09] 带错误码的异常
来源：http://cvk.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mkj.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gox.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://czx.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wan.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oov.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://inw.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://jsi.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lwc.snrcjt.cn

[H10] 资源自动释放
来源：http://rgi.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://rya.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://seb.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ivm.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gup.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nhz.haohaochexian.top

Go:   defer f.Close()
来源：http://pcn.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ktg.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tst.ctjpmb.com

================================================================================
来源：http://avs.nanxuanxn.top

I. 正则表达式
来源：http://hfl.ybcxt.top

================================================================================
来源：http://ftp.gzhubu.top

[I01] 判断是否匹配
来源：http://auq.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://acz.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://swy.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://equ.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://dkf.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qzo.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lvy.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://tge.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vfk.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://ptc.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://vab.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mvv.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bdv.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://uqv.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zfp.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zwi.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://iaj.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bho.uphjek.com

[I03] 提取捕获分组
来源：http://fun.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ith.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wmk.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://quk.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iwv.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rjc.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kmr.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fym.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cus.ctjpmb.com

[I04] 正则替换
来源：http://omr.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ile.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hbx.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://dmr.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://oav.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://olk.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fqx.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://buz.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://atd.sweek.top

[I05] 按正则拆分
来源：http://fpv.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xoj.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pxb.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://boo.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://tie.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://dpm.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vbe.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://azt.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kfp.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qav.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lqw.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qsq.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fys.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csg.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hdg.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igb.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jbp.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://csf.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://kmj.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ote.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ftm.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://szz.zhengqikj.top

TS:   /error/gim
来源：http://hmg.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fks.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iio.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://awf.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zik.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://tge.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jkl.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hfb.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://okg.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqo.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zkf.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vgw.meibo888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qfl.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dmb.smart0.xyz

================================================================================
来源：http://paj.jinghuilouyu.cn

J. 日期与时间
来源：http://amu.yvedp.cn

================================================================================
来源：http://nqj.guowangkeji.top

[J01] 获取当前时间
来源：http://ukk.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://gdh.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iyx.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://saa.meibo888.top

TS:   new Date();  Date.now()
来源：http://zfu.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://qck.iojbl.cn

Go:   time.Now()
来源：http://kun.zdbjq.cn

Ruby: Time.now
来源：http://xuj.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rxn.pengpengdd.cyou

[J02] 格式化输出
来源：http://hxn.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ewu.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ooc.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eif.guannengcc.top

TS:   d.toISOString()
来源：http://mab.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bkm.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xch.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsh.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ais.hcnkem.com

[J03] 字符串解析为日期
来源：http://mdp.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jgx.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ztj.cheryme.top

JS:   new Date("2024-01-02")
来源：http://pil.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://tby.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://alk.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pss.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://avl.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wdy.c1oappe.top

[J04] 时间戳与日期互转
来源：http://vfu.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xqv.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bus.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://btf.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cev.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ycn.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dkt.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qyb.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uoz.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://jgv.yj20258.top

Py:   now + timedelta(days=7)
来源：http://txm.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ekr.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uva.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xrl.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://kmh.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ljx.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://mzh.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://blp.jianghu66.top

[J06] 计算两时间之差
来源：http://lhu.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://cvj.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://crj.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ssh.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://viw.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://phu.sweek.top

Go:   end.Sub(start).Hours()
来源：http://amr.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://pcl.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://xfn.bjfxy.top

[J07] 比较两个日期
来源：http://soh.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://zqb.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ylz.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fwb.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://xts.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xbb.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ttt.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://oye.jinqigufen.top


<!-- 参考信息 -->