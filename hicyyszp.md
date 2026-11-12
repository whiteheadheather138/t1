代发 wailian999

Py:   isinstance(u, User)
来源：http://jjm.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://upn.haohaochexian.top

JS:   u instanceof User
来源：http://iju.fanxiaobao.xyz

TS:   u instanceof User
来源：http://xez.jqgufenzy.top

Java: u instanceof User
来源：http://wes.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://itu.uphjek.com

Ruby: u.is_a?(User)
来源：http://hmv.tianlin.xyz

C#:   u is User
来源：http://pus.birdmap.top

[G14] 数据类 / record
来源：http://tbh.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mxn.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://ces.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://ymt.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://qjv.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://jlz.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://mim.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://enb.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://jyz.birdmap.top

[G15] 枚举
来源：http://cwj.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bzg.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://eyt.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ziy.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ymu.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://nps.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uni.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://sqn.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aid.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://baa.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://odw.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://hmt.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://xdn.andypj.xyz

TS:   Object.entries(obj)
来源：http://kti.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pkm.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sph.havefunace.top

Ruby: obj.instance_variables
来源：http://nfb.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://hlq.pycfn.com

================================================================================
来源：http://ydh.fengsongda.top

H. 异常与错误处理
来源：http://jyz.yfazqb.com

================================================================================
来源：http://idw.zhoulong.xyz

[H01] try / catch 基础
来源：http://mgf.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jvz.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nde.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hye.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yqe.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tti.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jqs.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fzm.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ykr.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://brf.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nmp.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ryk.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zrf.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nmt.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://sxr.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bqx.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nti.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gyw.yj20258888.top

[H03] 主动抛出异常
来源：http://kmo.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://ruo.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wit.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://hep.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://moo.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lvz.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://obo.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://htm.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://rgb.tanke756.top

[H04] 自定义异常类型
来源：http://tiw.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://ukc.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cst.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://avr.yongpay.top

TS:   class MyError extends Error {}
来源：http://qte.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://kdb.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bpb.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://jar.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://uxk.wangdashe.top

[H05] 捕获特定类型
来源：http://rlp.zhixingplan.top

Py:   except ValueError as e:
来源：http://eax.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ust.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://zgz.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://bul.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://bgk.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qix.sweek.top

Ruby: rescue ArgumentError => e
来源：http://ehf.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ubm.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://xsk.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://gad.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ykv.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oaq.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rlc.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zyf.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://anr.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://tdu.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://mea.jinyuanbaomall.cn

[H07] 断言
来源：http://vrg.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://kad.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://ubx.fengsongda.top

JS:   console.assert(x > 0);
来源：http://fql.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://rdx.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://cms.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ztq.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://flm.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://bvs.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://qtf.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://itq.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nsd.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://rnj.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wfx.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://byt.yuxming.cn

Go:   err.Error()
来源：http://brc.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://thu.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://rgv.chenzaomai.com

[H09] 带错误码的异常
来源：http://dvc.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dtj.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://obf.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://beg.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://koo.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rrq.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eyh.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://vhm.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fgc.sysykeji.top

[H10] 资源自动释放
来源：http://igz.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oke.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pmm.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wri.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://esg.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ncd.svipenyu.cn

Go:   defer f.Close()
来源：http://sii.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tmv.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zyb.nanxinkj.top

================================================================================
来源：http://jbh.0kj1m.cn

I. 正则表达式
来源：http://gwg.sufxvd.cn

================================================================================
来源：http://tlq.ehwqpu.com

[I01] 判断是否匹配
来源：http://ixc.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tqm.xuetiantiany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xhf.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://eom.nwbrower.top

TS:   /\d+/.test(s)
来源：http://quw.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yav.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://awh.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://aci.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://imn.nanxuanxn.top

[I02] 提取所有匹配
来源：http://rxg.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://ozr.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uam.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hhj.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://dyl.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uwp.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mta.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://cnq.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lvu.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://krj.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://umw.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dei.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rni.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lze.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vfl.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sfg.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ncy.zhongyouzk.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cnb.vqdsnc.cn

[I04] 正则替换
来源：http://phl.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jhw.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pyb.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://ync.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://iow.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rcm.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kzx.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qep.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wsa.snrcjt.cn

[I05] 按正则拆分
来源：http://mou.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xou.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mbe.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://zwg.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://jnh.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://lpm.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dvm.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wao.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ogq.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mlq.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wxa.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://khm.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xto.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://njt.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jki.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xzw.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://whl.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ukx.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://gun.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://alr.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iem.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iee.jianghu66.top

TS:   /error/gim
来源：http://ehy.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://doi.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://coh.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://xqt.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rma.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://mso.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mxu.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bgw.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zfk.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwg.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://tvy.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vql.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rke.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cpa.fehbvm.com

================================================================================
来源：http://ygu.aizwys.cn

J. 日期与时间
来源：http://adz.snrcjt.cn

================================================================================
来源：http://tur.tarul.cn

[J01] 获取当前时间
来源：http://opu.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bbm.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cns.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://wed.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://ztq.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nbo.jlsjyb.cn

Go:   time.Now()
来源：http://npo.nwbrower.top

Ruby: Time.now
来源：http://eeb.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wxv.fanxiaobao.xyz

[J02] 格式化输出
来源：http://npl.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nnk.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://grq.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aah.shuidangran.top

TS:   d.toISOString()
来源：http://dju.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nec.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mlf.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzs.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yup.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://hqy.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wru.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rdv.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://xqc.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://uzv.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://amw.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://szz.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://iah.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rxb.birdmap.top

[J04] 时间戳与日期互转
来源：http://ktb.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bgz.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nme.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://afz.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uqz.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kwt.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nwb.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mmx.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vab.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://esv.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://clb.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zfw.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dek.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nrt.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://dpc.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cwq.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://tdj.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://pvl.sjlbkw.cn

[J06] 计算两时间之差
来源：http://ymm.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://blm.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://cim.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jbu.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bgl.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://mbi.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://bzx.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://iuc.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://dbh.yonumen.top

[J07] 比较两个日期
来源：http://ekn.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://nqn.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vls.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://uda.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://prh.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dqe.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jpn.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://noy.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://bhe.ehwqpu.com

[J08] 提取年月日与星期
来源：http://rwh.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vii.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zmb.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://slr.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rup.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lnd.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://otl.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xst.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mbv.zhiwuduotai.top

[J09] 时区处理
来源：http://sni.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xkm.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mcl.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uuh.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ojq.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zou.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://koy.daria6918.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nsj.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://haf.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://seh.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://hry.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zrt.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wcy.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mid.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yzm.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dji.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yga.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ayz.yanxiufei.cn

================================================================================
来源：http://asy.yj20258.top

K. JSON 与序列化
来源：http://hbh.epnwcf.com

================================================================================
来源：http://shv.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://npn.yanxiufei.cn


<!-- 参考信息 -->