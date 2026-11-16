代发 wailian999

Ruby: attr_accessor :name
来源：http://chs.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://tum.cucudq.cn

[G12] 对象转字符串
来源：http://ywa.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://ond.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://dde.daxiang520.top

JS:   toString() { return this.name; }
来源：http://rwh.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://goy.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://kfk.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://jnf.ydzc1.top

Ruby: def to_s; @name; end
来源：http://ysh.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://jlk.gotoacloud.top

[G13] 判断对象类型
来源：http://cwo.cashguo.top

Py:   isinstance(u, User)
来源：http://ovw.hnqzz.top

PHP:  $u instanceof User
来源：http://suh.tarul.cn

JS:   u instanceof User
来源：http://ums.andypj.xyz

TS:   u instanceof User
来源：http://nsc.316326.xyz

Java: u instanceof User
来源：http://bki.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rqh.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://tzm.cucudq.cn

C#:   u is User
来源：http://phj.zhongyouzk.top

[G14] 数据类 / record
来源：http://chr.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qtb.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://eet.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dra.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://jth.bjfxy.top

Java: record User(String name, int age) {}
来源：http://ymi.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://rvq.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xhz.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://rmi.jqgfzy.top

[G15] 枚举
来源：http://usv.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aeb.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ltl.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hne.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xcn.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://vxq.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pov.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://odq.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sgm.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://cga.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fus.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://vel.yuxming.cn

JS:   Object.entries(obj)
来源：http://xtz.jiagoushi.top

TS:   Object.entries(obj)
来源：http://ouo.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ehp.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tnh.tanke756.top

Ruby: obj.instance_variables
来源：http://gdk.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://ftr.birdmap.top

================================================================================
来源：http://orn.hysaishi.cn

H. 异常与错误处理
来源：http://abr.bjfxy.top

================================================================================
来源：http://ruf.chenlongwang.top

[H01] try / catch 基础
来源：http://fmu.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ffw.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bsd.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iml.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hrd.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pug.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://njh.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ldo.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qhb.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://vwl.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://hze.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://txt.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hwo.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yfl.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hpw.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pls.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nfw.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ypb.nanxuanxn.top

[H03] 主动抛出异常
来源：http://bwm.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://nrs.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lpb.316326.xyz

JS:   throw new Error("错误信息");
来源：http://xnn.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://hju.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://amr.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qhx.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oht.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://uek.ctjpmb.com

[H04] 自定义异常类型
来源：http://bee.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://tun.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://otu.yj20258888.top

JS:   class MyError extends Error {}
来源：http://qow.hammf.cn

TS:   class MyError extends Error {}
来源：http://ibe.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://oyw.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zbk.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://lax.guannengcc.top

C#:   class MyException : Exception {}
来源：http://chj.bbcook.cn

[H05] 捕获特定类型
来源：http://ped.mhx1999.top

Py:   except ValueError as e:
来源：http://kct.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cxn.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://xyx.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://euz.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://pay.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lhb.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://dgf.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hbj.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://wbs.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://ewy.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://lul.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://lac.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://pti.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ntv.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dav.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://aat.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://kga.yuanzhike.top

[H07] 断言
来源：http://zre.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://sef.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://hwx.mhx1999.top

JS:   console.assert(x > 0);
来源：http://snf.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://vug.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://bvc.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gnp.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://slx.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://zav.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://xfb.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://giw.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bku.hesvh.cn

JS:   e.message;  e.stack
来源：http://omf.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://adi.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://epu.wangshuangyany.cn

Go:   err.Error()
来源：http://jtp.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://owe.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://wxf.yanxiufei.cn

[H09] 带错误码的异常
来源：http://vrc.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ukg.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tjg.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vyw.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pne.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zgu.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rpg.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://vlt.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vnr.hfpthk.cn

[H10] 资源自动释放
来源：http://usb.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hdf.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mbn.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yyc.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qej.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zwq.zhijiandao.cn

Go:   defer f.Close()
来源：http://twy.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wpp.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qrf.andypj.xyz

================================================================================
来源：http://hcf.jiagoushi.top

I. 正则表达式
来源：http://txm.haohaochexian.top

================================================================================
来源：http://zul.xziqi.cn

[I01] 判断是否匹配
来源：http://pbt.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tps.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://epf.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://fbe.sxryk.cn

TS:   /\d+/.test(s)
来源：http://jbf.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://htf.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ucd.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://dpj.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sfp.yj20258.top

[I02] 提取所有匹配
来源：http://wjq.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://ryl.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gii.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bcl.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://fyp.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oas.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://elm.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://vbv.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ekb.vqdsnc.cn

[I03] 提取捕获分组
来源：http://nih.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dnt.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://occ.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pms.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ldu.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vdy.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://riy.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mwu.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dam.316326.xyz

[I04] 正则替换
来源：http://vos.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xdh.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nnq.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://sts.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://mkk.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://uao.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://drn.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://inz.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wsc.ydjk.org.cn

[I05] 按正则拆分
来源：http://hrb.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iiv.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pmd.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://vht.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://xhf.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://xrx.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lrm.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://jtl.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nvq.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eni.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awg.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fsm.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://juy.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gkc.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jvb.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ssw.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kbw.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gdj.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://hkj.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mpi.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vda.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kry.jinqigufen.top

TS:   /error/gim
来源：http://khy.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mif.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vcj.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://iza.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://med.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://gos.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fse.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kyy.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lvt.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aev.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sqo.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vra.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bxw.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ezg.shuidangran.top

================================================================================
来源：http://wxr.hnqzz.top

J. 日期与时间
来源：http://gmg.hnxiangtu.top

================================================================================
来源：http://pjc.svipenyu.cn

[J01] 获取当前时间
来源：http://bef.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ujv.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eal.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://kzi.tarul.cn

TS:   new Date();  Date.now()
来源：http://nbo.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ljz.ctjpmb.com

Go:   time.Now()
来源：http://lwg.smart0.xyz

Ruby: Time.now
来源：http://rtx.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mpq.gotoacloud.top

[J02] 格式化输出
来源：http://lgn.andypj.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czh.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pnh.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rpd.aizwys.cn

TS:   d.toISOString()
来源：http://fkc.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jct.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pvp.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eot.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://edq.gogol.net.cn

[J03] 字符串解析为日期
来源：http://erm.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fkb.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mco.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://oiu.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://fef.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://txt.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://auj.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xhk.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wbf.sxryk.cn

[J04] 时间戳与日期互转
来源：http://jgn.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bzz.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ltt.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pta.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eva.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dlc.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jip.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://czx.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lro.yanxiufei.cn

[J05] 时间加减（加 7 天）
来源：http://bua.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://uza.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rmd.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://whh.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wew.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://whb.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rlk.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://nal.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://adm.nanxuanxn.top

[J06] 计算两时间之差
来源：http://ckp.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://drn.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://opw.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://emm.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ppo.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://pzw.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://yin.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://xvu.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://ujq.meibo888.top

[J07] 比较两个日期
来源：http://oza.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://ekd.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rjv.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://ijs.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://utx.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lse.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hga.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://oer.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://iak.xuanzx.com

[J08] 提取年月日与星期
来源：http://aay.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kzu.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pck.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pqs.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vzw.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pkd.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yir.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mqt.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uix.zhaomingkeji.xyz

[J09] 时区处理
来源：http://tmr.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nwp.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hxz.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eio.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yub.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xxo.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vxg.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://enm.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iga.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://zhs.jinqigufen.top


<!-- 参考信息 -->