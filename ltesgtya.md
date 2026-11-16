代发 wailian999

JS:   get name() { return this._name; }
来源：http://gow.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://uel.snrcjt.cn

Java: public String getName() { return name; }
来源：http://vet.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://egl.tanke756.top

Ruby: attr_accessor :name
来源：http://hoq.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://pgu.quarkkingdee.top

[G12] 对象转字符串
来源：http://dyz.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://zcd.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xsq.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://zaz.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://wop.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://ske.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aqu.tanke756.top

Ruby: def to_s; @name; end
来源：http://wbu.316326.xyz

C#:   public override string ToString() => Name;
来源：http://pca.yueranfly.top

[G13] 判断对象类型
来源：http://aqa.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://hdq.aizwys.cn

PHP:  $u instanceof User
来源：http://mdh.mhx1999.top

JS:   u instanceof User
来源：http://efe.sysykeji.top

TS:   u instanceof User
来源：http://gna.snrcjt.cn

Java: u instanceof User
来源：http://off.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ljr.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://afd.ywan-chungtsiang.top

C#:   u is User
来源：http://ist.yuxming.cn

[G14] 数据类 / record
来源：http://dbg.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rbd.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://kig.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://opk.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://nnu.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://crb.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://jea.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jep.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://sor.cdnleiting.top

[G15] 枚举
来源：http://ayu.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nvq.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fvw.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xqx.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jkf.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://sjt.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nvj.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://iym.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hjd.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://mov.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://edz.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://zbh.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://buh.fzhhl.top

TS:   Object.entries(obj)
来源：http://bqk.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vrm.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://kyq.haohaochexian.top

Ruby: obj.instance_variables
来源：http://jrn.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://vfk.hysaishi.cn

================================================================================
来源：http://npk.nanxuanxn.top

H. 异常与错误处理
来源：http://ejz.guowangkeji.top

================================================================================
来源：http://chv.hcnkem.com

[H01] try / catch 基础
来源：http://hxm.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qce.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wdy.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bvn.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oex.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zje.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pbr.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://arr.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tee.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://chb.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ast.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://psv.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dgz.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jwk.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://jru.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ebn.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lwc.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ara.chenzaomai.com

[H03] 主动抛出异常
来源：http://xse.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://ajj.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mkc.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://qgs.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://cyh.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wsp.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rzt.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xky.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://zqo.wangdashe.top

[H04] 自定义异常类型
来源：http://tcp.hammf.cn

Py:   class MyError(Exception): pass
来源：http://gol.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://ryi.daria6918.cn

JS:   class MyError extends Error {}
来源：http://atz.yvedp.cn

TS:   class MyError extends Error {}
来源：http://twm.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://jjg.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://niu.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://wos.shuidangran.top

C#:   class MyException : Exception {}
来源：http://oju.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://ujc.ydzc1.top

Py:   except ValueError as e:
来源：http://toa.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lry.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://cgd.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://nkq.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://fmq.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jus.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://mcf.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cke.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://aub.cheryme.top

Py:   value = d.get("k") or default
来源：http://ndb.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tiy.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qln.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vcc.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uxd.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nxl.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://yqv.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://cki.nwbrower.top

[H07] 断言
来源：http://uwm.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://pef.hesvh.cn

PHP:  assert($x > 0);
来源：http://zec.guannengcc.top

JS:   console.assert(x > 0);
来源：http://bdr.yuanzhike.top

TS:   console.assert(x > 0);
来源：http://nox.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://vol.hysaishi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jjk.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jug.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://vlp.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://cry.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://npv.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vns.havefunace.top

JS:   e.message;  e.stack
来源：http://klj.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rba.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://udu.wangshuangyany.cn

Go:   err.Error()
来源：http://raz.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://xhj.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://bok.xziqi.cn

[H09] 带错误码的异常
来源：http://gyf.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://met.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pez.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wiq.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dwv.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://usy.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lmr.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vlm.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://sae.jinqigfzy.top

[H10] 资源自动释放
来源：http://umd.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zwf.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jmi.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hff.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pzm.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zqm.zhiwuduotai.top

Go:   defer f.Close()
来源：http://byc.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://omx.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wsk.jinqigfzy.top

================================================================================
来源：http://bgi.ivvv.top

I. 正则表达式
来源：http://coh.smart0.xyz

================================================================================
来源：http://gam.daria6918.cn

[I01] 判断是否匹配
来源：http://hge.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ipc.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://bmw.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://alq.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://jzx.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rko.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qwm.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://ugw.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vkx.zhixingplan.top

[I02] 提取所有匹配
来源：http://wxc.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://efc.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nck.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://phm.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://qqm.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tpk.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fnp.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://znn.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hjv.xylfe.cn

[I03] 提取捕获分组
来源：http://uut.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aos.sjlbkw.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qyq.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://myx.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xku.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ewz.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ulb.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ouv.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://snp.zhiwuduotai.top

[I04] 正则替换
来源：http://dni.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://llz.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fsy.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://vxp.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pfz.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://ect.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nce.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sdk.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vkj.cheryme.top

[I05] 按正则拆分
来源：http://nxu.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gsm.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xsj.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://ykc.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://lnr.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://xsi.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dio.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tyz.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ahs.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zsa.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://isr.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ljf.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujy.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://foy.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ati.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lys.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ouq.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vei.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://wtg.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://atn.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zpa.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ofd.ydjk.org.cn

TS:   /error/gim
来源：http://ekq.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ofk.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lrk.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://fpk.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgv.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://xdw.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://awm.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xhy.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://koa.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xtk.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://icv.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ktp.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vki.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cfw.zhaomingkeji.xyz

================================================================================
来源：http://dcn.chenlongwang.top

J. 日期与时间
来源：http://dwh.xziqi.cn

================================================================================
来源：http://oey.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://hgz.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ber.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zgj.epnwcf.com

JS:   new Date();  Date.now()
来源：http://vab.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://aed.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qjk.mhx1999.top

Go:   time.Now()
来源：http://ykp.vehdjk.com

Ruby: Time.now
来源：http://dzw.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://odm.yfazqb.com

[J02] 格式化输出
来源：http://etx.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lox.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hnn.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yaw.uphjek.com

TS:   d.toISOString()
来源：http://dbu.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xut.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tfv.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://khl.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qha.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://qiy.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qkc.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hts.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://zdt.ivvv.top

TS:   new Date("2024-01-02")
来源：http://pfq.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://kxb.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kmq.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://jwn.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cda.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://brq.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ubz.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://exg.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://doe.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ugl.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zmb.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://owm.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hen.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pez.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://mde.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://kxc.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sxu.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aua.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wcq.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://ooq.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ooa.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://xmt.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xum.meibo888.top

[J06] 计算两时间之差
来源：http://dwf.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://ffu.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://pct.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lcx.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vts.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://sur.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://get.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://yjf.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://nql.quarkkingdee.top

[J07] 比较两个日期
来源：http://uva.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://xlk.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://awr.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://bjz.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://ngg.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qcc.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://htv.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://wex.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://iyi.jyoumei.cn

[J08] 提取年月日与星期
来源：http://lco.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kfg.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lfx.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rnv.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hfn.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hpv.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ijg.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://may.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vxn.hammf.cn

[J09] 时区处理
来源：http://sxe.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qjd.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://czs.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wyq.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dxy.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qqw.tian-w.cn


<!-- 参考信息 -->