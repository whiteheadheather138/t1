代发 wailian999

Ruby: attr_accessor :name
来源：http://xeg.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://qrw.yj20258888.top

[G12] 对象转字符串
来源：http://ndb.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://smq.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://mlq.pycfn.com

JS:   toString() { return this.name; }
来源：http://sum.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://hgk.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://pyy.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cfb.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://vpy.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://nye.zhongyouzk.top

[G13] 判断对象类型
来源：http://cec.hywenlv.cn

Py:   isinstance(u, User)
来源：http://kbe.vqdsnc.cn

PHP:  $u instanceof User
来源：http://xqx.tarul.cn

JS:   u instanceof User
来源：http://hhb.fengsongda.top

TS:   u instanceof User
来源：http://bcj.shanyushiyangtech.top

Java: u instanceof User
来源：http://ttg.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://mlo.yonumen.top

Ruby: u.is_a?(User)
来源：http://tzi.vehdjk.com

C#:   u is User
来源：http://aqo.jianghu66.top

[G14] 数据类 / record
来源：http://nqm.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://due.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://vax.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://hok.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://vzl.hnqzz.top

Java: record User(String name, int age) {}
来源：http://klr.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://kyz.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hcy.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://tbq.shuidangran.top

[G15] 枚举
来源：http://kzx.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://evl.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cld.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kbo.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qho.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://lpw.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lsw.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://mtt.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cdh.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://qlc.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qzl.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://jlm.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://nbe.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://ccn.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jfq.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ndi.wangdashe.top

Ruby: obj.instance_variables
来源：http://bpj.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://lbq.aizwys.cn

================================================================================
来源：http://yby.redwolf501.top

H. 异常与错误处理
来源：http://gsr.svipenyu.cn

================================================================================
来源：http://iqe.chenjidiqi.icu

[H01] try / catch 基础
来源：http://dts.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fxi.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bxf.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pdd.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wza.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sea.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yeh.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dgp.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kyo.yfazqb.com

[H02] finally / ensure 收尾
来源：http://hkj.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://aio.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://olq.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://oio.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fyq.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://iye.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pck.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ilx.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rrf.c1oappe.top

[H03] 主动抛出异常
来源：http://iwq.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://mgk.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tdv.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://zjv.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://kpi.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aio.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lim.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://wmd.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://kzu.zhixingplan.top

[H04] 自定义异常类型
来源：http://ubu.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://rkl.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://czy.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://jky.sxryk.cn

TS:   class MyError extends Error {}
来源：http://gye.yuanzhike.top

Java: class MyException extends RuntimeException {}
来源：http://poi.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sxv.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://cjt.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://cku.cashguo.top

[H05] 捕获特定类型
来源：http://kxm.0kj1m.cn

Py:   except ValueError as e:
来源：http://gie.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kiw.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://qdb.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://qbp.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://mcd.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vqi.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://ijw.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lsd.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://chj.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://ltb.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://hxz.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://hdk.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://kbk.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mak.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ynw.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://dsh.jqgfzy.top

C#:   obj?.A?.B ?? default
来源：http://fjb.ybcxt.top

[H07] 断言
来源：http://vts.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://xsp.gotoacloud.top

PHP:  assert($x > 0);
来源：http://jer.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://mvo.yonumen.top

TS:   console.assert(x > 0);
来源：http://ptm.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://jtr.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rnw.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://qrw.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://ena.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://gvr.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://kzx.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pwn.nanxinkj.top

JS:   e.message;  e.stack
来源：http://hdk.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://xbq.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uxm.9152youxi.cn

Go:   err.Error()
来源：http://ntj.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://ucb.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://adp.zycfv.cn

[H09] 带错误码的异常
来源：http://oyj.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tdj.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jlg.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://buv.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tyu.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rbb.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cmf.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://ebg.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://dpv.gotoacloud.top

[H10] 资源自动释放
来源：http://doh.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://huk.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gsp.ehwqpu.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dtx.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://adp.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yge.yfazqb.com

Go:   defer f.Close()
来源：http://ujg.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tfb.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://idj.jinghuilouyu.cn

================================================================================
来源：http://hmz.xziqi.cn

I. 正则表达式
来源：http://oud.yj20258.top

================================================================================
来源：http://vxf.yj202588.top

[I01] 判断是否匹配
来源：http://mnk.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://edj.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://iwe.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://cly.hesvh.cn

TS:   /\d+/.test(s)
来源：http://fdp.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://chb.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yfu.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://iyt.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ozn.jiagoushi.top

[I02] 提取所有匹配
来源：http://lmf.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://mip.tanke756.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mes.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zuj.tanke756.top

TS:   s.match(/\d+/g)
来源：http://dbn.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sds.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tdx.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://ydb.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kks.jlsjyb.cn

[I03] 提取捕获分组
来源：http://htb.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kvd.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://djp.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hvg.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qwu.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hiz.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rpn.birdmap.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rgp.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uhv.iojbl.cn

[I04] 正则替换
来源：http://ojq.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wgz.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jnl.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://afw.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hin.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://cwh.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qqr.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xpy.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mvt.shuidangran.top

[I05] 按正则拆分
来源：http://ule.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rja.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qbp.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://isa.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://lmg.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://qin.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vgo.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ijm.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ipj.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hnx.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rox.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bjc.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dua.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ioc.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hxf.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vin.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bww.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bsz.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://sia.c1oappe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://elp.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wqt.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vcr.guannengcc.top

TS:   /error/gim
来源：http://bzu.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mmq.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://twf.yj20258.top

Ruby: s.scan(/error/i)
来源：http://vna.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://glx.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://yux.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sgl.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tsj.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cfn.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xmf.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uur.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://evx.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://skh.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hpk.snrcjt.cn

================================================================================
来源：http://vjl.jinyuanbaomall.cn

J. 日期与时间
来源：http://lnt.chenjidiqi.icu

================================================================================
来源：http://qhw.wangdashe.top

[J01] 获取当前时间
来源：http://eph.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wqy.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://onx.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://jfr.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://lln.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://slw.zhixingplan.top

Go:   time.Now()
来源：http://gdp.hnxiangtu.top

Ruby: Time.now
来源：http://wpc.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jem.dashuyun.cn

[J02] 格式化输出
来源：http://sta.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pjd.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hvy.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pbf.cashguo.top

TS:   d.toISOString()
来源：http://rku.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uyi.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ien.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://few.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://msq.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://oop.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://thi.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lao.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://gpw.tanke756.top

TS:   new Date("2024-01-02")
来源：http://vuo.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://sim.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fcz.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://rdu.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eaw.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://zds.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aip.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rtk.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wzp.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://msj.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ysa.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zsl.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbt.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xuc.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://ixp.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://qef.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://pjo.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wro.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://des.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://qym.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ehx.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://hvi.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://gwy.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://xbw.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://tff.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://hsg.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://loj.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jzp.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://snc.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://edb.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://zdj.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://whk.kuanghao11.cn

[J07] 比较两个日期
来源：http://ryv.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://csx.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ycs.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://iyd.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yrq.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vcu.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ysu.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://suz.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://wxp.havefunace.top

[J08] 提取年月日与星期
来源：http://zip.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mwl.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kyn.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wvf.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://umz.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://del.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ffd.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pcq.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vmo.ybcxt.top

[J09] 时区处理
来源：http://hra.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://scu.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cip.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gwo.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rin.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jex.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://daf.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hgq.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hhw.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://vcr.gaohongyu789.top


<!-- 参考信息 -->