代发 wailian999

Ruby: attr_accessor :name
来源：http://jlf.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://rqd.tarul.cn

[G12] 对象转字符串
来源：http://zth.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://kml.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pcx.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://jky.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://ife.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://zpg.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://fxz.fzhhl.top

Ruby: def to_s; @name; end
来源：http://kea.shzxlz.cn

C#:   public override string ToString() => Name;
来源：http://eds.aizwys.cn

[G13] 判断对象类型
来源：http://brk.hammf.cn

Py:   isinstance(u, User)
来源：http://htq.quarkkingdee.top

PHP:  $u instanceof User
来源：http://hnf.gotoacloud.top

JS:   u instanceof User
来源：http://iqk.jqgufenzy.top

TS:   u instanceof User
来源：http://oxt.redwolf501.top

Java: u instanceof User
来源：http://mfl.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://qfp.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://vzr.daria6918.cn

C#:   u is User
来源：http://yzi.nanxinkj.top

[G14] 数据类 / record
来源：http://ucl.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fql.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://enz.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lzp.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://xdz.yongpay.top

Java: record User(String name, int age) {}
来源：http://txr.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://ulm.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uuy.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://hgq.shangyingyoupin.top

[G15] 枚举
来源：http://osr.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kzq.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xzc.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nas.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ykt.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://ruo.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mxk.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://tpe.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pnt.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://mku.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bbo.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://kdm.chenlongwang.top

JS:   Object.entries(obj)
来源：http://gvv.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://tao.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uon.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hzu.yvedp.cn

Ruby: obj.instance_variables
来源：http://jyf.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://kst.yj20258.top

================================================================================
来源：http://ypf.zhongyouzk.top

H. 异常与错误处理
来源：http://stj.yanxiufei.cn

================================================================================
来源：http://bxt.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://gqv.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uws.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hgu.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dmt.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vxp.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nyc.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fsi.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vmn.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cum.wangdashe.top

[H02] finally / ensure 收尾
来源：http://rdg.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://jcw.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://qbh.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kgy.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mbx.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://owc.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://yrc.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ule.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://rdr.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://jrl.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://tso.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wwd.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://mem.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://zuj.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ilh.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://apr.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wim.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bcb.sufxvd.cn

[H04] 自定义异常类型
来源：http://uto.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://olj.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://psy.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://dvv.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://rjl.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://pev.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xph.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://zrd.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://nfk.cashguo.top

[H05] 捕获特定类型
来源：http://frl.nanxinkj.top

Py:   except ValueError as e:
来源：http://ibs.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lhy.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://cpx.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://vbg.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://asi.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dom.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://nxo.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ngh.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://qtp.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://zye.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://ltm.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://mhk.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://icz.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dms.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://mzk.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://dva.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://njf.wangshuangyany.cn

[H07] 断言
来源：http://xqw.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://pzc.hesvh.cn

PHP:  assert($x > 0);
来源：http://zre.hnqzz.top

JS:   console.assert(x > 0);
来源：http://pkz.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://zra.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://okt.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zuq.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vbo.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://ivl.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://huw.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://sod.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kjv.bjfxy.top

JS:   e.message;  e.stack
来源：http://wdo.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hpi.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ylm.ybcxt.top

Go:   err.Error()
来源：http://jlr.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://pam.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://nyl.quarkkingdee.top

[H09] 带错误码的异常
来源：http://hfk.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yjb.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yud.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nea.dashuyun.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vno.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kag.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ilo.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://zhc.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yzc.vehdjk.com

[H10] 资源自动释放
来源：http://iaa.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rwa.tarul.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ych.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qzd.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lvl.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ome.epnwcf.com

Go:   defer f.Close()
来源：http://bld.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qrq.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://del.xuetiantiany.cn

================================================================================
来源：http://cku.sjlbkw.cn

I. 正则表达式
来源：http://wvv.jinqigfzy.top

================================================================================
来源：http://fus.jiagoushi.top

[I01] 判断是否匹配
来源：http://bre.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ihd.tianlin.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://gmf.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://zsd.yuxming.cn

TS:   /\d+/.test(s)
来源：http://kbw.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fhp.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oyx.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://srl.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://heh.ydzc1.top

[I02] 提取所有匹配
来源：http://rjj.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://bsg.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jpu.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://idr.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://iyg.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iso.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nhu.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://bte.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gjs.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://xny.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lwe.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rlc.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lqm.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sga.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aqh.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lct.tarul.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xtj.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dav.wangshuangyany.cn

[I04] 正则替换
来源：http://vhy.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gfn.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://csy.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://muy.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://zrf.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yyi.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://eva.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zjz.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://alw.jyoumei.cn

[I05] 按正则拆分
来源：http://abe.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zfk.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vnu.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://drp.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://ytb.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://fnc.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gqr.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://myc.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eno.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rzm.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eek.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jbz.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://alq.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sgg.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ifx.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vvb.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oxx.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ced.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://fmv.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fye.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wff.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://okf.feifeiyinyue.top

TS:   /error/gim
来源：http://zrz.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ujm.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qqd.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://lju.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hwu.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://mxt.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jgk.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mxw.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zbl.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hfb.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://exr.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://otl.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xdq.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vxf.yvedp.cn

================================================================================
来源：http://ufb.aibaodan.cn

J. 日期与时间
来源：http://vyi.bbcook.cn

================================================================================
来源：http://xfp.yuanzhike.top

[J01] 获取当前时间
来源：http://jwd.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xvt.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cdt.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://zvy.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://cku.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bje.quarkkingdee.top

Go:   time.Now()
来源：http://yip.daria6918.cn

Ruby: Time.now
来源：http://jys.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yzt.9152youxi.cn

[J02] 格式化输出
来源：http://ivm.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vst.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hgv.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ime.ydjk.org.cn

TS:   d.toISOString()
来源：http://rnn.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vtt.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://efp.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nuy.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pwm.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://nok.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dab.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://shx.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://kpy.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://hxq.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jur.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://klj.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://nzq.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qsy.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://wms.aibaodan.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pfx.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dwx.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tko.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://acb.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ovb.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xhl.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zim.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xdh.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://gec.havefunace.top

Py:   now + timedelta(days=7)
来源：http://eeo.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sgv.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aqu.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://evm.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://npb.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lsw.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://pqq.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://bmr.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://sgt.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://xzx.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://rlk.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ues.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://evl.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://vei.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://ahy.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://xfn.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://uqf.hnqzz.top

[J07] 比较两个日期
来源：http://avw.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://fxd.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yzw.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dum.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://efk.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jgs.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ojh.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://bcv.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://xzy.gogol.net.cn

[J08] 提取年月日与星期
来源：http://qos.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mjq.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rud.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cjd.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hcf.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blx.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wqo.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ejk.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xha.daria6918.cn

[J09] 时区处理
来源：http://bvz.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uhc.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nwf.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tfy.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kym.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yqs.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tct.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://zhm.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tso.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://igz.hammf.cn


<!-- 参考信息 -->