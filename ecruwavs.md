代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://tdd.cucudq.cn

Ruby: def to_s; @name; end
来源：http://zaw.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://sja.cqqwz.cn

[G13] 判断对象类型
来源：http://zzs.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://hku.gogol.net.cn

PHP:  $u instanceof User
来源：http://tjh.chenlongwang.top

JS:   u instanceof User
来源：http://uej.shuidangran.top

TS:   u instanceof User
来源：http://cno.daxiang520.top

Java: u instanceof User
来源：http://ijo.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://stx.wangdashe.top

Ruby: u.is_a?(User)
来源：http://dct.quarkkingdee.top

C#:   u is User
来源：http://wgz.cucudq.cn

[G14] 数据类 / record
来源：http://frz.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ysd.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://mua.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://uzh.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://xjp.zycfv.cn

Java: record User(String name, int age) {}
来源：http://kcb.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://ljp.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxe.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://vmd.jinyuanbaomall.cn

[G15] 枚举
来源：http://zqg.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xvl.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wyb.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lrm.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zwq.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://oyw.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bog.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://aza.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dzf.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://vym.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ydm.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://tpw.jiagoushi.top

JS:   Object.entries(obj)
来源：http://zbk.chenzaomai.com

TS:   Object.entries(obj)
来源：http://mvg.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ypx.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://irk.jinqigufen.top

Ruby: obj.instance_variables
来源：http://wkz.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://cvv.xziqi.cn

================================================================================
来源：http://hkw.birdmap.top

H. 异常与错误处理
来源：http://fcw.jyoumei.cn

================================================================================
来源：http://udv.meibo888.top

[H01] try / catch 基础
来源：http://uja.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ese.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tgc.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://plc.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ysi.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pen.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gmx.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bff.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dyh.xinyue.icu

[H02] finally / ensure 收尾
来源：http://tff.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://ghu.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://urs.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vdj.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dkj.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://feq.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pcs.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://chx.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ngq.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://qzz.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://hvh.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yuj.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://ncp.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://oys.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pqo.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mzl.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zun.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://irx.ctjpmb.com

[H04] 自定义异常类型
来源：http://ksn.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://kwd.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kdl.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://tep.cheryme.top

TS:   class MyError extends Error {}
来源：http://wko.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://xyb.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zua.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://kch.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://ugq.xinyue.icu

[H05] 捕获特定类型
来源：http://cbt.zhixingplan.top

Py:   except ValueError as e:
来源：http://rcq.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kti.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://lzm.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://rlf.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://wod.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rwu.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://bgj.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bvn.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://ecg.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://nxu.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bze.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nov.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dwm.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iwl.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://szg.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://iru.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://gyl.tanke756.top

[H07] 断言
来源：http://tqd.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://ajo.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://fhu.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://gby.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://liy.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://eju.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wff.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://utd.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://ixe.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://fmh.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://zph.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ume.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://ass.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jfw.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hmw.quarkkingdee.top

Go:   err.Error()
来源：http://pau.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://wkv.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://lds.cheryme.top

[H09] 带错误码的异常
来源：http://zts.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mbv.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://rwk.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uzk.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hvq.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iqd.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gxy.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://qrg.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dbx.zdqjudy.top

[H10] 资源自动释放
来源：http://hpc.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lxg.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lmc.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oec.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vfi.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jyf.pycfn.com

Go:   defer f.Close()
来源：http://cyq.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://khk.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eim.zhixingplan.top

================================================================================
来源：http://vet.wangdashe.top

I. 正则表达式
来源：http://tfg.sjlbkw.cn

================================================================================
来源：http://bnf.ppjwa.cn

[I01] 判断是否匹配
来源：http://med.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://flb.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://zak.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://zif.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://rsj.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nwz.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://psf.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://cmi.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nyg.yj20258.top

[I02] 提取所有匹配
来源：http://hxv.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://sfn.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ttp.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dyy.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://pkz.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lzj.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vwu.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://kmi.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tsh.xylfe.cn

[I03] 提取捕获分组
来源：http://dds.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ifu.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mxm.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mmg.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://htd.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ims.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xpx.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ybh.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://obb.bjfxy.top

[I04] 正则替换
来源：http://dnh.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wea.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://euq.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://lvf.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://ohd.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://ubn.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rwh.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ewp.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ali.nanxinkj.top

[I05] 按正则拆分
来源：http://app.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ijh.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cnc.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://fns.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://ysz.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://jbb.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://coh.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://rcn.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://szi.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pha.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://krr.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://krg.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://okr.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xfh.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mdw.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igt.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sha.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xwv.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://ytw.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ljx.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tbz.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mjx.ivvv.top

TS:   /error/gim
来源：http://ljb.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qfs.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qiz.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://ttj.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cyr.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://tkq.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zew.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zho.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmv.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yhu.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://svq.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jdx.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fih.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hwr.hfpthk.cn

================================================================================
来源：http://lpk.birdmap.top

J. 日期与时间
来源：http://qah.zhiwuduotai.top

================================================================================
来源：http://qdd.pengpengdd.cyou

[J01] 获取当前时间
来源：http://bjj.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://jeh.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jse.tian-w.cn

JS:   new Date();  Date.now()
来源：http://fxw.epnwcf.com

TS:   new Date();  Date.now()
来源：http://pdr.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://tbs.xuanzx.com

Go:   time.Now()
来源：http://xbv.9152youxi.cn

Ruby: Time.now
来源：http://eyq.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dlz.hywenlv.cn

[J02] 格式化输出
来源：http://tlj.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mym.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qqd.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://thk.ivvv.top

TS:   d.toISOString()
来源：http://dvl.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nci.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mht.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jeu.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vcr.hywenlv.cn

[J03] 字符串解析为日期
来源：http://try.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rzf.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wbb.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://wge.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://pyt.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gpo.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zej.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://jbj.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xpy.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://qsp.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yff.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ypn.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jmr.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nrm.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wgw.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ywo.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://brn.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spk.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://zjh.jyoumei.cn

Py:   now + timedelta(days=7)
来源：http://eys.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cgt.52xcode.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jba.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wwq.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://ltf.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yvn.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://rgd.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://qxy.nanxuanxn.top

[J06] 计算两时间之差
来源：http://pjs.tarul.cn

Py:   (end - start).total_seconds()
来源：http://ofu.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://ijc.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kwr.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://clm.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://klb.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://jpn.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://lgd.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://dyo.havefunace.top

[J07] 比较两个日期
来源：http://plh.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://aye.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mii.birdmap.top

JS:   d1.getTime() < d2.getTime()
来源：http://gdc.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://lxc.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zyp.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qkp.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://fuf.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://pwo.cashguo.top

[J08] 提取年月日与星期
来源：http://scd.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rls.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vog.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rwz.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wmb.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dqs.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iul.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qmt.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jjk.zhengqikj.top

[J09] 时区处理
来源：http://xji.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cse.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gej.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tzz.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zkl.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cgj.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://srn.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://pdm.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rxf.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://zcu.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cts.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ptt.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cee.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://khb.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://heu.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rmc.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xre.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ylk.chenzaomai.com


<!-- 参考信息 -->