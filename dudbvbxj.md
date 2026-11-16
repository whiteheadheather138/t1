代发 wailian999

[G14] 数据类 / record
来源：http://yoj.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vos.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://gub.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://ynb.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://bam.shuidangran.top

Java: record User(String name, int age) {}
来源：http://tse.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://qfo.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cqz.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://kic.c1oappe.top

[G15] 枚举
来源：http://ukd.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wea.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uos.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://osa.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://spc.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://klm.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dex.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://ega.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fne.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://cnp.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vtl.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://voq.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://nxu.chenzaomai.com

TS:   Object.entries(obj)
来源：http://zsv.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gmo.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nqm.bjfxy.top

Ruby: obj.instance_variables
来源：http://ekm.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://jkw.wangshuangyany.cn

================================================================================
来源：http://hqq.zhiwuduotai.top

H. 异常与错误处理
来源：http://cvu.zhongyouzk.top

================================================================================
来源：http://ukh.yvedp.cn

[H01] try / catch 基础
来源：http://lry.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xfl.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vpx.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zcr.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nbm.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ars.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xbt.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://msk.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rkm.birdmap.top

[H02] finally / ensure 收尾
来源：http://ntq.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ssw.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://thk.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ljp.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vsu.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hbv.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zmy.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vdf.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rrk.guowangkeji.top

[H03] 主动抛出异常
来源：http://ifw.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://oxx.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wjr.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://fcr.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://sfb.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xha.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sue.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://key.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://kml.fktsv.cn

[H04] 自定义异常类型
来源：http://zae.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://pxn.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://nvz.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://nyt.hammf.cn

TS:   class MyError extends Error {}
来源：http://dcn.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://nsr.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xdt.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://aud.andypj.xyz

C#:   class MyException : Exception {}
来源：http://vth.yj202588.top

[H05] 捕获特定类型
来源：http://mxl.cheryme.top

Py:   except ValueError as e:
来源：http://wcq.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pvg.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://trj.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://maj.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://chk.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cyx.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://hwf.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eoz.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://zet.birdmap.top

Py:   value = d.get("k") or default
来源：http://qdg.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://cps.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://qsz.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kmq.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://opz.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ceo.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://iaj.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://wjj.snrcjt.cn

[H07] 断言
来源：http://nuj.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://fde.hywenlv.cn

PHP:  assert($x > 0);
来源：http://ord.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://hfe.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://elf.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://zpq.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tyd.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cge.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://riz.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://vae.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://lli.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fce.sysykeji.top

JS:   e.message;  e.stack
来源：http://vsk.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rda.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pvz.hysaishi.cn

Go:   err.Error()
来源：http://drx.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://llp.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://bqt.pycfn.com

[H09] 带错误码的异常
来源：http://bmb.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iev.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fti.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wfj.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ayj.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://krd.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ibk.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://nji.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ysp.hammf.cn

[H10] 资源自动释放
来源：http://sdv.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wzj.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mkv.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sfy.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nuh.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wuv.c1oappe.top

Go:   defer f.Close()
来源：http://zlg.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vbo.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iav.ywan-chungtsiang.top

================================================================================
来源：http://lhs.ywan-chungtsiang.top

I. 正则表达式
来源：http://ggc.yonumen.top

================================================================================
来源：http://grz.yueranfly.top

[I01] 判断是否匹配
来源：http://jse.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zbn.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kmr.ydzc1.top

JS:   /\d+/.test(s)
来源：http://xaq.mhx1999.top

TS:   /\d+/.test(s)
来源：http://umw.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fao.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pdk.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://maf.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qbh.zhixingplan.top

[I02] 提取所有匹配
来源：http://jpr.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://ofi.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xpt.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://enp.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://evh.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xzj.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://guq.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://sbf.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ndk.bjfxy.top

[I03] 提取捕获分组
来源：http://vpk.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bga.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pin.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ycr.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dbn.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tzw.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpn.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xwz.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cwt.52xcode.cn

[I04] 正则替换
来源：http://pwe.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rji.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vby.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://zcw.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://frb.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fzk.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zvb.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ruj.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://juz.redwolf501.top

[I05] 按正则拆分
来源：http://mks.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://cow.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://avl.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://yvg.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://fkq.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://ccj.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ykc.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://tuw.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rmb.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ixn.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://clq.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zfd.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ktm.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ebp.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pvi.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uiu.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ubx.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://okp.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://cfd.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xcx.tianlin.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nou.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://elg.dashuyun.cn

TS:   /error/gim
来源：http://sen.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rgf.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://niv.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://hyv.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dnu.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://xlp.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cyy.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jla.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tom.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gqi.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mtv.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://act.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://upi.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lvg.meibo888.top

================================================================================
来源：http://zmn.jyoumei.cn

J. 日期与时间
来源：http://vdb.birdmap.top

================================================================================
来源：http://ycb.hongshengwenyu.top

[J01] 获取当前时间
来源：http://gsw.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dky.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://grj.yfazqb.com

JS:   new Date();  Date.now()
来源：http://dww.cashguo.top

TS:   new Date();  Date.now()
来源：http://bqr.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hny.hysaishi.cn

Go:   time.Now()
来源：http://xbk.wangdashe.top

Ruby: Time.now
来源：http://pci.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kan.yanxiufei.cn

[J02] 格式化输出
来源：http://ijp.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wkf.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qud.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kvf.aizwys.cn

TS:   d.toISOString()
来源：http://dpc.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dzt.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://phf.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfl.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fxi.zdbjq.cn

[J03] 字符串解析为日期
来源：http://lpe.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qkr.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cxl.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://tuz.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://nzc.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://sfd.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vhu.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://tdy.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lky.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://itz.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bgc.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rjd.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cjf.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dhm.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ecv.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hxp.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vbi.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bcd.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://dcf.cheryme.top

Py:   now + timedelta(days=7)
来源：http://rjl.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tcp.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzl.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mcn.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://ffy.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hln.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://mem.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rcc.bjfxy.top

[J06] 计算两时间之差
来源：http://bef.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://lyi.sweek.top

PHP:  $end->diff($start)->days;
来源：http://arr.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vvr.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xmr.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://cqp.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://ehd.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://wve.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://xxz.yvedp.cn

[J07] 比较两个日期
来源：http://lkr.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://saj.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://emf.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://qfv.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pek.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://toa.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://klh.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://fgo.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://tzh.cdnleiting.top

[J08] 提取年月日与星期
来源：http://ddi.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fhq.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tij.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hmf.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bbh.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qpu.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kye.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://daw.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hub.fanxiaobao.xyz

[J09] 时区处理
来源：http://nka.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ndq.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hnb.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oyj.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://typ.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://urn.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pfl.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zii.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ciz.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://dov.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xpo.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://spv.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ifm.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://odk.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://whw.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ztf.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hru.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gtf.0kj1m.cn

================================================================================
来源：http://aou.nwbrower.top

K. JSON 与序列化
来源：http://srl.guowangkeji.top

================================================================================
来源：http://lhl.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://jyt.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mkk.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xmp.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://oce.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://teq.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hzx.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://uvy.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ahh.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://flt.dashuyun.cn


<!-- 参考信息 -->