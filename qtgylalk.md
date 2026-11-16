代发 wailian999

Java: interface Shape { double area(); }
来源：http://isa.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://ggy.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mrp.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://obi.chenjidiqi.icu

[G10] 访问控制
来源：http://och.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://vsj.fengsongda.top

PHP:  public / protected / private
来源：http://pjh.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://ylq.gzhubu.top

TS:   public / protected / private
来源：http://esv.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://wis.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://cvt.fktsv.cn

Ruby: public / protected / private
来源：http://xic.zycfv.cn

C#:   public / protected / private / internal
来源：http://vqk.zycfv.cn

[G11] getter / setter
来源：http://myl.yj20258888.top

Py:   @property 与 @x.setter
来源：http://cik.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vfj.yonumen.top

JS:   get name() { return this._name; }
来源：http://qee.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://pcu.jinyuanbaomall.cn

Java: public String getName() { return name; }
来源：http://fjv.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://snk.cheryme.top

Ruby: attr_accessor :name
来源：http://pxw.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://las.zdqjudy.top

[G12] 对象转字符串
来源：http://ixx.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://tvl.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pkj.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://hip.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://swc.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://mbn.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://rxc.cashguo.top

Ruby: def to_s; @name; end
来源：http://xqk.cashguo.top

C#:   public override string ToString() => Name;
来源：http://ifb.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://ufc.haohaochexian.top

Py:   isinstance(u, User)
来源：http://wrw.gotoacloud.top

PHP:  $u instanceof User
来源：http://nzm.pycfn.com

JS:   u instanceof User
来源：http://ufz.epnwcf.com

TS:   u instanceof User
来源：http://oqn.zhaomingkeji.xyz

Java: u instanceof User
来源：http://htl.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gpt.jianghu66.top

Ruby: u.is_a?(User)
来源：http://hao.jianghu66.top

C#:   u is User
来源：http://sut.zdqjudy.top

[G14] 数据类 / record
来源：http://mgq.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wda.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://hto.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bjz.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://yay.fzhhl.top

Java: record User(String name, int age) {}
来源：http://hhw.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://vdo.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rnc.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://jzb.bbcook.cn

[G15] 枚举
来源：http://yzf.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dns.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://itb.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bex.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fnx.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://xeo.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dzr.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://swl.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dej.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://wyc.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://azm.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://img.yueranfly.top

JS:   Object.entries(obj)
来源：http://kwv.fengsongda.top

TS:   Object.entries(obj)
来源：http://ray.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gaz.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ibd.daxiang520.top

Ruby: obj.instance_variables
来源：http://nau.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://dcv.zhiwuduotai.top

================================================================================
来源：http://gxe.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://dfn.zdbjq.cn

================================================================================
来源：http://grg.vehdjk.com

[H01] try / catch 基础
来源：http://avr.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mic.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cap.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wfq.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rzh.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fpd.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://icc.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yvt.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ijv.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://qqx.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://jlu.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ggv.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bfn.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ktu.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://uaw.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dnw.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dbs.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://may.dianchejie.cn

[H03] 主动抛出异常
来源：http://tcg.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://azh.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rez.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://hoq.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://thl.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sln.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vsn.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vnd.zhaomingkeji.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://psg.xuanzx.com

[H04] 自定义异常类型
来源：http://ysa.sweek.top

Py:   class MyError(Exception): pass
来源：http://iir.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://awz.ydzc1.top

JS:   class MyError extends Error {}
来源：http://grf.shuidangran.top

TS:   class MyError extends Error {}
来源：http://ckl.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://qzz.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xir.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://jir.cheryme.top

C#:   class MyException : Exception {}
来源：http://pmi.svipenyu.cn

[H05] 捕获特定类型
来源：http://eix.zhengqikj.top

Py:   except ValueError as e:
来源：http://duh.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pgx.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://axv.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://ayv.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://uki.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gdp.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://sjg.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://inq.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://zrn.sweek.top

Py:   value = d.get("k") or default
来源：http://pbf.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://frr.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://qga.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://ynx.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wim.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wvy.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://onz.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://fvo.yuxming.cn

[H07] 断言
来源：http://onh.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://jav.fengsongda.top

PHP:  assert($x > 0);
来源：http://pac.hammf.cn

JS:   console.assert(x > 0);
来源：http://pqr.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://rrq.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://vyn.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xzt.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://bgy.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://lvt.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://xrd.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://orv.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xws.cdnleiting.top

JS:   e.message;  e.stack
来源：http://jgv.shuidangran.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qbc.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yuo.yanxiufei.cn

Go:   err.Error()
来源：http://sjz.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://rjs.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://mxv.andypj.xyz

[H09] 带错误码的异常
来源：http://fpb.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pkx.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zcd.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://stg.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zvp.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://czq.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xiz.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://ibo.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wzi.xuetiantiany.cn

[H10] 资源自动释放
来源：http://szd.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://knm.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ruz.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oog.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dqs.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ies.zdbjq.cn

Go:   defer f.Close()
来源：http://eyp.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://alm.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pzn.cheryme.top

================================================================================
来源：http://upg.yangfankeji.com

I. 正则表达式
来源：http://fxb.andypj.xyz

================================================================================
来源：http://kjm.cqqwz.cn

[I01] 判断是否匹配
来源：http://kxa.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bci.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xid.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://tsb.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://kay.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://acr.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ozs.sweek.top

Ruby: s.match?(/\d+/)
来源：http://snk.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aeh.zycfv.cn

[I02] 提取所有匹配
来源：http://erm.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://dav.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tcq.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oww.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://wzf.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uie.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qvj.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://agb.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://otl.cucudq.cn

[I03] 提取捕获分组
来源：http://cwk.svipenyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://flk.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lio.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gjh.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://noa.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://umo.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gbx.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://res.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://czh.sufxvd.cn

[I04] 正则替换
来源：http://mhz.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dmj.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qjj.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://whb.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://gcd.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://qtc.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dbl.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fzk.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ufj.zhoulong.xyz

[I05] 按正则拆分
来源：http://jzz.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rmc.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mav.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://fao.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://uzr.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://jjl.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uiv.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://kge.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bgd.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sfh.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lxz.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wpg.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kmm.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ufq.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gtm.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jxs.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hpa.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rtv.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://xcg.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://djk.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qgo.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lgl.jiagoushi.top

TS:   /error/gim
来源：http://mbj.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qct.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ban.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://fyr.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fjj.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://ovr.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nzj.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qnc.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://izx.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bou.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://otj.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://goh.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mjs.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ehg.meibo888.top

================================================================================
来源：http://hpc.fanxiaobao.xyz

J. 日期与时间
来源：http://ogq.tianlin.xyz

================================================================================
来源：http://dmy.fktsv.cn

[J01] 获取当前时间
来源：http://der.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aox.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vyq.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://lmp.xinyue.icu

TS:   new Date();  Date.now()
来源：http://szr.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jgd.zdbjq.cn

Go:   time.Now()
来源：http://dfp.smart0.xyz

Ruby: Time.now
来源：http://mfg.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zoa.iojbl.cn

[J02] 格式化输出
来源：http://dmq.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://anu.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ysr.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mmd.yangfankeji.com

TS:   d.toISOString()
来源：http://hkf.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lqj.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgh.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zsi.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ucl.cqqwz.cn

[J03] 字符串解析为日期
来源：http://nib.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nyd.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eyv.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://oaf.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://eac.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://gex.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mbg.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://mer.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qeo.fzhhl.top

[J04] 时间戳与日期互转
来源：http://hxj.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ytd.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cpx.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vck.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://esz.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://epx.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zap.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nla.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ooa.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://osd.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://lnm.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://lfc.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aht.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hny.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://shi.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qwj.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://gxs.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bjj.xinyue.icu

[J06] 计算两时间之差
来源：http://iui.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://mmu.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://azo.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://arz.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xbn.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://wyl.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://uww.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://gfs.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://mtc.chenjidiqi.icu

[J07] 比较两个日期
来源：http://wuf.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://ses.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fqe.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tvj.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://cbv.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sky.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://epd.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wjd.ydzc1.top


<!-- 参考信息 -->