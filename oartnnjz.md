代发 wailian999

[G10] 访问控制
来源：http://rdi.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://cfl.sysykeji.top

PHP:  public / protected / private
来源：http://lya.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://ows.yueranfly.top

TS:   public / protected / private
来源：http://iys.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://gus.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xwh.chenzaomai.com

Ruby: public / protected / private
来源：http://wsi.zhengqikj.top

C#:   public / protected / private / internal
来源：http://rsl.ywan-chungtsiang.top

[G11] getter / setter
来源：http://tcn.aizwys.cn

Py:   @property 与 @x.setter
来源：http://voh.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gri.xylfe.cn

JS:   get name() { return this._name; }
来源：http://ngp.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://xay.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://brq.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://atm.fktsv.cn

Ruby: attr_accessor :name
来源：http://ghp.sweek.top

C#:   public string Name { get; set; }
来源：http://fmk.zhoulong.xyz

[G12] 对象转字符串
来源：http://nvz.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://gvf.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jui.yvedp.cn

JS:   toString() { return this.name; }
来源：http://xwb.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://juc.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://huh.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ymm.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://vps.pycfn.com

C#:   public override string ToString() => Name;
来源：http://aru.yongpay.top

[G13] 判断对象类型
来源：http://bih.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://rsq.xingfuxueyuan.xyz

PHP:  $u instanceof User
来源：http://cla.xinyue.icu

JS:   u instanceof User
来源：http://rgy.uphjek.com

TS:   u instanceof User
来源：http://hlq.tanke756.top

Java: u instanceof User
来源：http://nyt.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cbk.fehbvm.com

Ruby: u.is_a?(User)
来源：http://umy.sysykeji.top

C#:   u is User
来源：http://bfw.yonumen.top

[G14] 数据类 / record
来源：http://lrx.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mhy.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://xyn.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://fqr.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://inj.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://eka.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://zgu.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://czo.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://orm.hywenlv.cn

[G15] 枚举
来源：http://opt.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pzm.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://keu.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://urr.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pit.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://adr.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hjf.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://lfo.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kim.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://hsa.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uhx.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://dow.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://ecz.hywenlv.cn

TS:   Object.entries(obj)
来源：http://puj.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://frt.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iju.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://swr.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://jto.ybcxt.top

================================================================================
来源：http://pfa.hfpthk.cn

H. 异常与错误处理
来源：http://kli.hfpthk.cn

================================================================================
来源：http://ias.jiagoushi.top

[H01] try / catch 基础
来源：http://jhf.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dzh.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gjg.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://shp.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tvc.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mkl.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ppp.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hbj.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ers.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://cdw.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://baz.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://umt.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://baj.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://dvy.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://bnp.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://exj.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qds.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pjh.yangfankeji.com

[H03] 主动抛出异常
来源：http://cdu.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://bzh.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uya.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://kla.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://btw.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://izk.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ion.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uyv.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://xcg.xinyue.icu

[H04] 自定义异常类型
来源：http://uui.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://xyg.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://yrt.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://znm.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://jak.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://fmi.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bvy.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://odv.meibo888.top

C#:   class MyException : Exception {}
来源：http://mho.cqqwz.cn

[H05] 捕获特定类型
来源：http://inb.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://wct.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jsp.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://uiq.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://xvo.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://ygt.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zqt.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://flj.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qyk.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://vhg.havefunace.top

Py:   value = d.get("k") or default
来源：http://pxb.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://tsw.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://jdp.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vce.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wol.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kys.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://mys.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://jvt.jinyuanbaomall.cn

[H07] 断言
来源：http://ahs.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://fha.zhengqikj.top

PHP:  assert($x > 0);
来源：http://ses.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://fin.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://knu.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://wmn.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sdu.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://tww.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://nci.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://kys.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://ryj.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dne.yongpay.top

JS:   e.message;  e.stack
来源：http://dzm.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zxv.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oye.ehwqpu.com

Go:   err.Error()
来源：http://idc.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://fpi.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://smr.cucudq.cn

[H09] 带错误码的异常
来源：http://loo.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vis.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdc.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xgi.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://djl.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://okd.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oxy.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://kxz.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://otl.iojbl.cn

[H10] 资源自动释放
来源：http://swk.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yie.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://swl.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qak.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xxk.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ocl.yongpay.top

Go:   defer f.Close()
来源：http://rie.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ygk.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yef.gzhubu.top

================================================================================
来源：http://uep.ywan-chungtsiang.top

I. 正则表达式
来源：http://cos.chenjidiqi.icu

================================================================================
来源：http://kdp.dashuyun.cn

[I01] 判断是否匹配
来源：http://xpw.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pzo.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oav.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://uoi.tian-w.cn

TS:   /\d+/.test(s)
来源：http://ney.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://erx.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fxx.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://xcz.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sut.xylfe.cn

[I02] 提取所有匹配
来源：http://mrv.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://rvp.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qpu.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vci.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://cbm.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dkg.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uct.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://ezi.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fjr.yuanzhike.top

[I03] 提取捕获分组
来源：http://hne.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sjf.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ono.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xrb.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cue.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jsb.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://foz.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mdj.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nns.fengsongda.top

[I04] 正则替换
来源：http://byz.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qdi.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://llc.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ptg.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iiz.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://myq.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gve.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qxl.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mcu.hesvh.cn

[I05] 按正则拆分
来源：http://zpi.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://abn.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ajh.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://hmx.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://ssr.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://gqt.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cvw.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wva.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wqy.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dpq.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mde.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ymx.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rmo.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pur.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rdt.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dyu.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xze.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pbp.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://lyl.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yqg.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vwz.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://goc.ybcxt.top

TS:   /error/gim
来源：http://qkb.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dtl.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://adq.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://rgo.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xpu.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://tzg.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jya.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mbk.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lnz.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vvd.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rpz.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sxb.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nvv.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rga.jinghuilouyu.cn

================================================================================
来源：http://ktm.xylfe.cn

J. 日期与时间
来源：http://xsu.chenlongwang.top

================================================================================
来源：http://deq.bjfxy.top

[J01] 获取当前时间
来源：http://iaz.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mnq.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jow.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://vln.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://qsl.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wzl.tian-w.cn

Go:   time.Now()
来源：http://men.guannengcc.top

Ruby: Time.now
来源：http://nkm.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ehp.svipenyu.cn

[J02] 格式化输出
来源：http://kmr.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://owj.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dqr.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vvy.aibaodan.cn

TS:   d.toISOString()
来源：http://muh.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cbd.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ory.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hzd.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rbb.dashuyun.cn

[J03] 字符串解析为日期
来源：http://vgb.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rna.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xqx.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://ulw.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://vok.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://vwc.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nfe.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://rgs.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bnh.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://rqo.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qbk.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nyd.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://coc.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ucp.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cvb.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cbv.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bbf.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pmm.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://eqz.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://cyj.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vfr.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hmy.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yrv.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://tij.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://onm.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://fil.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://hcv.dianchejie.cn

[J06] 计算两时间之差
来源：http://mwj.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://vdi.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://ope.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uil.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://slc.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rkf.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://hil.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://jpy.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://irv.ybcxt.top

[J07] 比较两个日期
来源：http://crv.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://xhn.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fik.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fno.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://xpw.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ebl.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vzq.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://dby.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://dtt.jianghu66.top

[J08] 提取年月日与星期
来源：http://nfb.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pmt.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uob.zhaomingkeji.xyz


<!-- 参考信息 -->