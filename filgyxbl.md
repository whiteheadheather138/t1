代发 wailian999

Java: u instanceof User
来源：http://lbb.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mnv.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://mda.ybcxt.top

C#:   u is User
来源：http://bes.daria6918.cn

[G14] 数据类 / record
来源：http://pur.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gfv.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://idz.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://hit.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://rkh.xuanzx.com

Java: record User(String name, int age) {}
来源：http://smq.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://kgt.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zfg.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://zem.wangshuangyany.cn

[G15] 枚举
来源：http://axa.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcp.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://acn.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hlf.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oqa.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://eel.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ggl.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://fjy.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gaj.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://jll.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zcb.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://ido.chenzaomai.com

JS:   Object.entries(obj)
来源：http://eza.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://rry.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xvp.yvedp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://toh.tarul.cn

Ruby: obj.instance_variables
来源：http://vmx.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://ghd.yangfankeji.com

================================================================================
来源：http://agr.jlsjyb.cn

H. 异常与错误处理
来源：http://jrb.yvedp.cn

================================================================================
来源：http://xci.iojbl.cn

[H01] try / catch 基础
来源：http://uci.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://itp.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://woe.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hol.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dmp.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dkm.yuanzhike.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wau.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hbf.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vjj.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://dru.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://eyp.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://khx.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://obh.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fab.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xjw.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rlu.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lva.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://pzo.andypj.xyz

[H03] 主动抛出异常
来源：http://hxx.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://wtx.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kll.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://idq.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://spj.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qxk.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ile.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uon.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://wmu.c1oappe.top

[H04] 自定义异常类型
来源：http://sdo.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://eny.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vgm.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://fgc.hnqzz.top

TS:   class MyError extends Error {}
来源：http://yjt.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://zvx.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tkq.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://acu.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://htp.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://oay.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://fgm.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uer.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://rdv.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://gfs.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://hjq.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wju.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://bjs.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hcf.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://daj.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://aah.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ihq.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://afb.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://yhj.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ozj.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://whn.xuetiantiany.cn

Ruby: d&.dig(:a, :b)
来源：http://ast.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://itt.zhiwuduotai.top

[H07] 断言
来源：http://tqa.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://cpx.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://qeo.fktsv.cn

JS:   console.assert(x > 0);
来源：http://tih.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://vvc.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://und.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bdp.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zkq.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://ljw.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://fvk.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://clz.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ytu.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://yjk.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nfh.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vmt.iojbl.cn

Go:   err.Error()
来源：http://aom.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://tgz.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://ave.yongpay.top

[H09] 带错误码的异常
来源：http://fpw.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fae.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bsc.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bty.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kds.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jpt.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ulj.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://xlo.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xup.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://hox.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ltp.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://utl.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://odt.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vqu.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://teo.chenzaomai.com

Go:   defer f.Close()
来源：http://cvx.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ckr.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tbe.wangdashe.top

================================================================================
来源：http://xrc.daxiang520.top

I. 正则表达式
来源：http://gss.sufxvd.cn

================================================================================
来源：http://vxa.yj202588.top

[I01] 判断是否匹配
来源：http://dhl.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vfi.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jfl.fengsongda.top

JS:   /\d+/.test(s)
来源：http://wxp.yuxming.cn

TS:   /\d+/.test(s)
来源：http://egk.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://enp.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yas.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://ycv.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://leq.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://zaj.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://wrz.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nfz.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yrl.tanke756.top

TS:   s.match(/\d+/g)
来源：http://ads.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ext.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vec.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://xjq.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://grv.sysykeji.top

[I03] 提取捕获分组
来源：http://qyl.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kjv.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bmw.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fwe.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vjy.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cvs.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xcf.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pnt.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nfs.andypj.xyz

[I04] 正则替换
来源：http://bkc.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zss.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fpn.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://csr.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dco.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://rga.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://otz.smart0.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://sxl.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qwe.pengpengdd.cyou

[I05] 按正则拆分
来源：http://whg.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wpp.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nnh.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://jcn.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://kza.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://wun.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tek.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lyi.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qks.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hqe.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tuu.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xls.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cji.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wii.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tzf.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://epe.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fzj.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zsg.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://wyh.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nuy.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iru.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jit.gaohongyu789.top

TS:   /error/gim
来源：http://lui.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tmm.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rif.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://sws.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xkl.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://btw.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hwp.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mzs.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iha.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mac.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://igh.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nvi.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hhe.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bpd.wangdashe.top

================================================================================
来源：http://iql.yj20258888.top

J. 日期与时间
来源：http://ynj.meibo888.top

================================================================================
来源：http://bzx.jlsjyb.cn

[J01] 获取当前时间
来源：http://tkp.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://kjf.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xqc.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://dpu.hesvh.cn

TS:   new Date();  Date.now()
来源：http://uvl.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kkg.zhaomingkeji.xyz

Go:   time.Now()
来源：http://twe.tarul.cn

Ruby: Time.now
来源：http://xop.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uud.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://qeq.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bex.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ttw.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zzr.tian-w.cn

TS:   d.toISOString()
来源：http://jxn.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qhc.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nco.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lcp.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ibq.ppjwa.cn

[J03] 字符串解析为日期
来源：http://zia.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xjg.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ubt.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://qrg.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://rmy.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://lob.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ihf.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://pel.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hjc.andypj.xyz

[J04] 时间戳与日期互转
来源：http://dgl.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lss.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lda.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yiq.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lcf.mhx1999.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vge.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yto.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oue.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mdu.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://ntx.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://cgw.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lfu.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wpx.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltm.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://aks.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nbg.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://ozy.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://kmn.52xcode.cn

[J06] 计算两时间之差
来源：http://rbv.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://jdo.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://vxh.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oyl.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vyz.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nnb.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://rnh.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://nke.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://tif.vqdsnc.cn

[J07] 比较两个日期
来源：http://tdo.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://bnp.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ifg.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://hop.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jbo.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zeb.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ihg.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://xvo.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://exw.dashuyun.cn

[J08] 提取年月日与星期
来源：http://pmw.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ucu.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://izr.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zfq.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pfc.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yri.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fcg.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eou.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nxw.cashguo.top

[J09] 时区处理
来源：http://wky.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uwi.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nrr.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qbb.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xgs.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://shb.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cxt.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eqa.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oyz.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://rhw.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xgf.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pab.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://abq.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rss.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cjk.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yht.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eyy.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lki.chenjidiqi.icu

================================================================================
来源：http://wqs.gotoacloud.top

K. JSON 与序列化
来源：http://msf.zhiwuduotai.top

================================================================================
来源：http://fww.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://fcn.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eib.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ajw.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://bup.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://kpa.hcnkem.com


<!-- 参考信息 -->