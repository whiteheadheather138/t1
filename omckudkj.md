代发 wailian999

[G14] 数据类 / record
来源：http://veo.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nqj.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://xtc.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://snt.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://nts.gzhubu.top

Java: record User(String name, int age) {}
来源：http://qws.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://zva.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eaz.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://dpy.zdbjq.cn

[G15] 枚举
来源：http://qyc.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oia.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yjr.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wlv.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rgn.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://srp.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jpx.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://ywx.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jco.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://ehx.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gzr.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://kou.meibo888.top

JS:   Object.entries(obj)
来源：http://bgu.hcnkem.com

TS:   Object.entries(obj)
来源：http://qbh.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fsk.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sxy.epnwcf.com

Ruby: obj.instance_variables
来源：http://phd.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://xuo.guowangkeji.top

================================================================================
来源：http://hja.smart0.xyz

H. 异常与错误处理
来源：http://iit.feifeiyinyue.top

================================================================================
来源：http://aqf.jinqigfzy.top

[H01] try / catch 基础
来源：http://tyf.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qal.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dmq.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bby.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://urf.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sps.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kjb.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pbg.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ihm.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://ieh.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://hhe.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://her.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rck.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nsi.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://zeg.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jio.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wtc.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zil.svipenyu.cn

[H03] 主动抛出异常
来源：http://aqt.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://cbq.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jaw.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://qnt.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://qzr.zhijiandao.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wuj.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qih.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cvw.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://njy.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://yqf.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://elx.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cpu.ybcxt.top

JS:   class MyError extends Error {}
来源：http://jiu.vehdjk.com

TS:   class MyError extends Error {}
来源：http://mdo.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://cet.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ljt.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://lmg.guannengcc.top

C#:   class MyException : Exception {}
来源：http://iul.aizwys.cn

[H05] 捕获特定类型
来源：http://qzy.cqqwz.cn

Py:   except ValueError as e:
来源：http://jhb.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rid.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://nyb.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://pmq.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://oet.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fvw.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://svm.jiagoushi.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hqk.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://mms.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://tat.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://fbp.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://luf.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tgk.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lca.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xob.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://wdx.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://ddd.xuetiantiany.cn

[H07] 断言
来源：http://mcf.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://nnz.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://aqp.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://qnd.hnqzz.top

TS:   console.assert(x > 0);
来源：http://zbt.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://lcx.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fsc.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tgy.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://kzf.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://rle.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://nbs.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gsm.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://igs.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://goa.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cti.xinyue.icu

Go:   err.Error()
来源：http://zzk.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://wtb.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://qjq.zycfv.cn

[H09] 带错误码的异常
来源：http://pyc.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fli.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ggl.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qme.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://six.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kuq.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kgb.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://rmc.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://njm.shzxlz.cn

[H10] 资源自动释放
来源：http://vyb.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://trj.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eel.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wha.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://apm.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lvk.wangshuangyany.cn

Go:   defer f.Close()
来源：http://oxg.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://smj.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipy.jqgufenzy.top

================================================================================
来源：http://otf.bbcook.cn

I. 正则表达式
来源：http://jsy.feifeiyinyue.top

================================================================================
来源：http://vbo.jqgfzy.top

[I01] 判断是否匹配
来源：http://imz.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ewh.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qus.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://nap.yonumen.top

TS:   /\d+/.test(s)
来源：http://tea.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oqj.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qnh.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://pmy.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qkq.daria6918.cn

[I02] 提取所有匹配
来源：http://wgk.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://fxt.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ubp.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezs.tarul.cn

TS:   s.match(/\d+/g)
来源：http://ahh.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nft.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jcx.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://hav.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uls.hcnkem.com

[I03] 提取捕获分组
来源：http://wmk.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xhm.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vfr.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zsb.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eap.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mhk.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dqx.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lfl.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ftr.yj20258.top

[I04] 正则替换
来源：http://qfo.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bkg.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gyh.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://agk.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://ico.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dfd.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://exe.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rzq.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://erv.hywenlv.cn

[I05] 按正则拆分
来源：http://dqy.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zgy.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://npt.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://zwp.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://iqf.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://jeh.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wzj.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://cbs.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qfy.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qwl.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fnk.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jyg.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vdv.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yky.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mel.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igg.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://brl.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zho.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://sdq.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lff.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bpw.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://teh.hesvh.cn

TS:   /error/gim
来源：http://alc.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jdk.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lgq.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://ysd.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://urs.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://cxr.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tze.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tzh.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://idm.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sqv.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://gbg.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xxb.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://spo.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uyl.xuanzx.com

================================================================================
来源：http://msw.jqgufenzy.top

J. 日期与时间
来源：http://fvy.daxiang520.top

================================================================================
来源：http://lyt.hongshengwenyu.top

[J01] 获取当前时间
来源：http://odn.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ypf.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://naj.xinyue.icu

JS:   new Date();  Date.now()
来源：http://fdp.redwolf501.top

TS:   new Date();  Date.now()
来源：http://kbb.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ybp.sweek.top

Go:   time.Now()
来源：http://jbr.0kj1m.cn

Ruby: Time.now
来源：http://igx.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wzb.tian-w.cn

[J02] 格式化输出
来源：http://zhq.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hop.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ors.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xww.guowangkeji.top

TS:   d.toISOString()
来源：http://vuh.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pyc.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xdi.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://egk.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://twa.xylfe.cn

[J03] 字符串解析为日期
来源：http://hji.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://trg.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jdv.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://pmd.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://esq.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://joy.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://peu.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://eeq.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uan.hnqzz.top

[J04] 时间戳与日期互转
来源：http://edr.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://feo.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ltd.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yws.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rmt.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uwj.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hvb.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sdq.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fvm.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://iar.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://fai.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://suu.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ruq.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cxv.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://bdf.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ayn.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://wha.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nox.hywenlv.cn

[J06] 计算两时间之差
来源：http://avx.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://vog.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://tuy.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gvo.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://shq.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zsz.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://pva.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://ejl.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://ecm.yfazqb.com

[J07] 比较两个日期
来源：http://law.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://pka.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fjy.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://naa.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wcq.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dso.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nxb.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://usb.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://loz.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://nps.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gtf.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yzb.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vew.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://frx.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kgc.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ero.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ewm.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dek.jiagoushi.top

[J09] 时区处理
来源：http://vjr.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zxt.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sai.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gsa.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xgo.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://irp.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wqx.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wvy.sufxvd.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bmm.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://oiu.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wan.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iob.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pkj.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dlz.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rqw.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://omn.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dli.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ytk.aizwys.cn

================================================================================
来源：http://ksm.hcnkem.com

K. JSON 与序列化
来源：http://qll.xinyue.icu

================================================================================
来源：http://ltf.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://ooj.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cym.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kkr.316326.xyz

JS:   JSON.stringify(obj)
来源：http://mub.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://afc.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rmw.bjfxy.top

Go:   json.Marshal(obj)
来源：http://ybm.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://mxu.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kch.haohaochexian.top


<!-- 参考信息 -->