代发 wailian999

Java: interface Shape { double area(); }
来源：http://szm.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://ksw.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jot.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://byp.jyoumei.cn

[G10] 访问控制
来源：http://euj.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://ltq.guannengcc.top

PHP:  public / protected / private
来源：http://ydu.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://dom.yanxiufei.cn

TS:   public / protected / private
来源：http://snq.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://pmk.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mvp.jinqigufen.top

Ruby: public / protected / private
来源：http://deb.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://ioa.cdnleiting.top

[G11] getter / setter
来源：http://pzy.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://rqg.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mwc.fengsongda.top

JS:   get name() { return this._name; }
来源：http://ewk.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://zvg.zdbjq.cn

Java: public String getName() { return name; }
来源：http://sjl.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qcv.cucudq.cn

Ruby: attr_accessor :name
来源：http://bqg.mhx1999.top

C#:   public string Name { get; set; }
来源：http://jqt.zhiwuduotai.top

[G12] 对象转字符串
来源：http://jzm.cheryme.top

Py:   def __str__(self): return self.name
来源：http://dyr.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://icr.redwolf501.top

JS:   toString() { return this.name; }
来源：http://xak.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://jse.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://eab.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jan.andypj.xyz

Ruby: def to_s; @name; end
来源：http://qxd.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://hnk.tarul.cn

[G13] 判断对象类型
来源：http://opq.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://odi.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://sie.dashuyun.cn

JS:   u instanceof User
来源：http://ptr.yuxming.cn

TS:   u instanceof User
来源：http://ktg.zdbjq.cn

Java: u instanceof User
来源：http://rnm.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kwy.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://xam.mhx1999.top

C#:   u is User
来源：http://xne.jinqigufen.top

[G14] 数据类 / record
来源：http://jsh.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bsu.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://aob.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://edy.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://mlj.pycfn.com

Java: record User(String name, int age) {}
来源：http://tta.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://dec.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ggz.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://ktk.hcnkem.com

[G15] 枚举
来源：http://ump.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jnr.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://khr.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sry.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mci.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://zxw.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kqg.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://tds.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://slv.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://tna.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fmd.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://ges.ydzc1.top

JS:   Object.entries(obj)
来源：http://czc.cucudq.cn

TS:   Object.entries(obj)
来源：http://qvf.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pra.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://cqp.nanxinkj.top

Ruby: obj.instance_variables
来源：http://lbp.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://sqc.yj202588.top

================================================================================
来源：http://fym.52xcode.cn

H. 异常与错误处理
来源：http://smm.jinyuanbaomall.cn

================================================================================
来源：http://ghv.zhongyouzk.top

[H01] try / catch 基础
来源：http://xla.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wtw.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nhg.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qla.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qjd.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://atn.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wlx.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ewp.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zpe.hcnkem.com

[H02] finally / ensure 收尾
来源：http://sxl.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://fdb.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wwz.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vdm.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lhp.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tlf.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mnr.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://maq.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ere.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://ivg.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://tfw.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qje.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://ccg.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://kkx.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://wni.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://liw.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wpp.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://zig.zdbjq.cn

[H04] 自定义异常类型
来源：http://cmt.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://emt.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pqj.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://ogy.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://bsg.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://xpf.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qbj.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://wgh.mhx1999.top

C#:   class MyException : Exception {}
来源：http://fdf.dashuyun.cn

[H05] 捕获特定类型
来源：http://vag.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://han.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://knr.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://jrm.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://wqa.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://dek.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kgy.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://hir.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://whg.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://egv.tanke756.top

Py:   value = d.get("k") or default
来源：http://pdi.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://kcm.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ojc.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://cus.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ofk.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dym.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://buu.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://bwx.jqgfzy.top

[H07] 断言
来源：http://dgy.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://nsy.cucudq.cn

PHP:  assert($x > 0);
来源：http://var.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://wsb.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://wyt.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://vrt.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://umo.yuanzhike.top

Ruby: raise "必须为正" unless x > 0
来源：http://llt.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://noh.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://fqm.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://ans.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mwa.andypj.xyz

JS:   e.message;  e.stack
来源：http://hyx.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://and.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fvw.zycfv.cn

Go:   err.Error()
来源：http://pez.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://xhx.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://fdb.zhijiandao.cn

[H09] 带错误码的异常
来源：http://gvw.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oqc.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vkf.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://skl.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lhp.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kvt.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fri.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rba.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ycm.nanxuanxn.top

[H10] 资源自动释放
来源：http://wxd.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mis.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rlz.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xpy.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uso.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fsq.hfpthk.cn

Go:   defer f.Close()
来源：http://ydc.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zyb.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xqr.zhengqikj.top

================================================================================
来源：http://djq.mhx1999.top

I. 正则表达式
来源：http://vjg.gzhubu.top

================================================================================
来源：http://wgz.jyoumei.cn

[I01] 判断是否匹配
来源：http://tpz.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tec.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://hud.tarul.cn

JS:   /\d+/.test(s)
来源：http://ynt.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://kyk.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ova.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://epj.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://iwe.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eer.wangdashe.top

[I02] 提取所有匹配
来源：http://ibj.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://zzo.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pbu.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kea.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://shk.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mzt.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dtu.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://irz.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ltk.shzxlz.cn

[I03] 提取捕获分组
来源：http://abj.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rez.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ett.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tum.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ahj.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://upz.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xqj.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lsi.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vwk.fengsongda.top

[I04] 正则替换
来源：http://lta.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://sqm.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tyl.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ajc.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://viw.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wzr.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://yoy.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://npi.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tjb.xuanzx.com

[I05] 按正则拆分
来源：http://mvl.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mxe.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://etd.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://mut.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://ekp.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://xdf.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lwm.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://nez.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hwt.meibo888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rrt.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfq.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://elw.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jtn.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://anz.chenjidiqi.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rsa.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mqp.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hyj.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mwa.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://osh.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bwg.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lph.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kqk.zhoulong.xyz

TS:   /error/gim
来源：http://afv.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yiv.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rey.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://quh.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wqz.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://uoi.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://klc.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zvj.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dlw.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gqd.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rex.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ypo.gzhubu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jar.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mlv.sweek.top

================================================================================
来源：http://qhw.cucudq.cn

J. 日期与时间
来源：http://ddh.redwolf501.top

================================================================================
来源：http://res.ybcxt.top

[J01] 获取当前时间
来源：http://xfz.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hpl.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ejo.smart0.xyz

JS:   new Date();  Date.now()
来源：http://hvj.fzhhl.top

TS:   new Date();  Date.now()
来源：http://jix.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hnv.cqqwz.cn

Go:   time.Now()
来源：http://dit.xylfe.cn

Ruby: Time.now
来源：http://cbr.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wrh.gotoacloud.top

[J02] 格式化输出
来源：http://eni.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzx.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yjp.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qof.xuetiantiany.cn

TS:   d.toISOString()
来源：http://pyj.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ikv.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hbf.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://upg.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hfx.sufxvd.cn

[J03] 字符串解析为日期
来源：http://xjy.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fio.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpt.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://zrf.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://crb.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://cit.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kdo.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://kje.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cqm.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://dwc.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rir.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mgk.zhoulong.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://awd.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vty.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aos.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cws.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oda.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hmg.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://sts.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://edi.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://noe.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ihe.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://stx.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://ixw.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jiy.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://twg.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://ion.sxryk.cn

[J06] 计算两时间之差
来源：http://rul.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://jlq.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://lzd.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gbb.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eaq.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://ftv.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://ilp.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://qde.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://bso.52xcode.cn

[J07] 比较两个日期
来源：http://ohh.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://yiy.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dmc.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://vir.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://tga.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vsn.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kpd.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://yvs.jinqigfzy.top


<!-- 参考信息 -->