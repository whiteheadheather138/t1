代发 wailian999

Java: interface Shape { double area(); }
来源：http://pel.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://ggb.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rce.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://fju.haohaochexian.top

[G10] 访问控制
来源：http://kwy.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://deg.yfazqb.com

PHP:  public / protected / private
来源：http://fqz.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://rli.sweek.top

TS:   public / protected / private
来源：http://cdb.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://zde.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tel.vqdsnc.cn

Ruby: public / protected / private
来源：http://azs.ctjpmb.com

C#:   public / protected / private / internal
来源：http://ykx.fengsongda.top

[G11] getter / setter
来源：http://sbc.cucudq.cn

Py:   @property 与 @x.setter
来源：http://orf.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://amt.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://ide.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://hkx.316326.xyz

Java: public String getName() { return name; }
来源：http://icb.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ouy.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://xcp.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://snf.andypj.xyz

[G12] 对象转字符串
来源：http://zbl.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://azq.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lsi.yj20258.top

JS:   toString() { return this.name; }
来源：http://uns.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://agd.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://got.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lzv.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://gsu.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://hec.nwbrower.top

[G13] 判断对象类型
来源：http://fuq.yj20258.top

Py:   isinstance(u, User)
来源：http://axd.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://uxa.cdnleiting.top

JS:   u instanceof User
来源：http://enq.yueranfly.top

TS:   u instanceof User
来源：http://lrz.guannengcc.top

Java: u instanceof User
来源：http://ywz.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ppk.xuanzx.com

Ruby: u.is_a?(User)
来源：http://uuh.chenzaomai.com

C#:   u is User
来源：http://oju.sjlbkw.cn

[G14] 数据类 / record
来源：http://qcf.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fci.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://ysp.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://van.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://esg.guannengcc.top

Java: record User(String name, int age) {}
来源：http://uic.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://ruy.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wtq.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://zfn.hnxiangtu.top

[G15] 枚举
来源：http://eqj.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oyz.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ffk.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fnx.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ruk.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://bzd.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xna.chenjidiqi.icu

Ruby: Color = %i[red green].freeze
来源：http://trk.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bti.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://ics.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mad.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://yyu.havefunace.top

JS:   Object.entries(obj)
来源：http://pwg.feifeiyinyue.top

TS:   Object.entries(obj)
来源：http://tfs.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uoy.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lie.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://qkv.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://ylq.bbcook.cn

================================================================================
来源：http://deh.kuanghao11.cn

H. 异常与错误处理
来源：http://jla.hesvh.cn

================================================================================
来源：http://qhk.shzxlz.cn

[H01] try / catch 基础
来源：http://bjm.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aso.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fwz.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://war.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gjc.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://unb.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kfw.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zso.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kxp.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://hon.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fgl.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vdd.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tsh.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mle.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://ujq.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zql.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nff.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ubq.zhijiandao.cn

[H03] 主动抛出异常
来源：http://cga.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://rry.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sca.yj20258.top

JS:   throw new Error("错误信息");
来源：http://ahk.fzhhl.top

TS:   throw new Error("错误信息");
来源：http://sdi.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fun.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cpi.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://dms.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://ztw.c1oappe.top

[H04] 自定义异常类型
来源：http://gww.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://rlb.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://beg.yvedp.cn

JS:   class MyError extends Error {}
来源：http://mjg.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://poi.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://leb.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sfg.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://vje.guannengcc.top

C#:   class MyException : Exception {}
来源：http://ecr.yuanzhike.top

[H05] 捕获特定类型
来源：http://oap.haohaochexian.top

Py:   except ValueError as e:
来源：http://knw.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jqk.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://rwl.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://uqn.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://vav.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yaj.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://vee.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cys.yongpay.top

[H06] 可选值 / 空值安全访问
来源：http://nwu.tian-w.cn

Py:   value = d.get("k") or default
来源：http://rqi.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ysk.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://akp.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gxv.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fqa.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xhj.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://axb.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://euf.dianchejie.cn

[H07] 断言
来源：http://wwh.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://pnb.zdqjudy.top

PHP:  assert($x > 0);
来源：http://miw.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://qxe.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://mod.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://inh.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mfm.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://cue.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://vrc.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://iwq.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://xhf.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xdm.nwbrower.top

JS:   e.message;  e.stack
来源：http://wsy.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zdj.hysaishi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://myt.ctjpmb.com

Go:   err.Error()
来源：http://tkj.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://yoo.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://ncw.sysykeji.top

[H09] 带错误码的异常
来源：http://afn.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iyz.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://reu.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qzf.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://riq.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kml.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://giu.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cyc.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://swg.ybcxt.top

[H10] 资源自动释放
来源：http://bch.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://jkv.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iab.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rla.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hhi.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pus.chenzaomai.com

Go:   defer f.Close()
来源：http://kkv.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jjy.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://upi.nwbrower.top

================================================================================
来源：http://gmz.fanxiaobao.xyz

I. 正则表达式
来源：http://poz.hywenlv.cn

================================================================================
来源：http://nvl.zycfv.cn

[I01] 判断是否匹配
来源：http://wir.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://icv.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://wpn.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://eek.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://hzs.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ske.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qhs.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://rxb.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yld.nwbrower.top

[I02] 提取所有匹配
来源：http://uxd.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://yfx.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://njt.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zzs.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://hor.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://skn.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tpk.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://jta.gotoacloud.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wye.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://ett.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rik.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://skl.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vur.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pvc.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://noa.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dra.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tjx.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://asj.kuanghao11.cn

[I04] 正则替换
来源：http://qom.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xjn.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xwp.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fcg.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nxl.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rdr.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://spw.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nfk.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qhj.hnqzz.top

[I05] 按正则拆分
来源：http://fbg.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://yzu.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ywu.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ebc.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://jzu.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://soc.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tjm.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://jlu.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://opl.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vgu.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://anb.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://txl.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://emd.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://goj.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kls.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gbc.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vkl.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://awa.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://keu.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uha.yongpay.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eji.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pqp.tian-w.cn

TS:   /error/gim
来源：http://syp.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://crw.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cxn.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://rlx.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sqa.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://iwt.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oel.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ojq.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vpw.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gll.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hpk.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hlm.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uhe.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aca.jiagoushi.top

================================================================================
来源：http://ufc.tianlin.xyz

J. 日期与时间
来源：http://dqg.jyoumei.cn

================================================================================
来源：http://doq.jlsjyb.cn

[J01] 获取当前时间
来源：http://ixc.yonumen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dwj.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vbi.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://hoo.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://ivb.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nkd.gzhubu.top

Go:   time.Now()
来源：http://xuw.zhijiandao.cn

Ruby: Time.now
来源：http://wpe.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rhu.xuetiantiany.cn

[J02] 格式化输出
来源：http://jps.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nvx.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bsb.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cbi.ehwqpu.com

TS:   d.toISOString()
来源：http://rwo.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pac.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kgg.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cjy.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hyh.shuidangran.top

[J03] 字符串解析为日期
来源：http://cyu.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://upu.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pud.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://uya.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://soo.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://bkb.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tnt.guowangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://wvl.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://weh.yfazqb.com

[J04] 时间戳与日期互转
来源：http://jpn.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xpq.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ufw.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wpe.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jqv.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ekz.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pln.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://alr.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hko.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://mrj.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://ird.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uts.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zyi.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vgn.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://dzy.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jvq.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://llw.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://acz.gaohongyu789.top

[J06] 计算两时间之差
来源：http://zxo.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://fvn.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://wwm.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://flp.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ouw.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ouu.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://hmj.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://qry.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://fsb.fktsv.cn

[J07] 比较两个日期
来源：http://izo.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://biz.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dnv.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wwx.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rjr.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://thv.shanyushiyangtech.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://opl.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vrl.meibo888.top


<!-- 参考信息 -->