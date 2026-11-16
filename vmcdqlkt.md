代发 wailian999

Java: u instanceof User
来源：http://jlo.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fts.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://tlk.hysaishi.cn

C#:   u is User
来源：http://buv.yongpay.top

[G14] 数据类 / record
来源：http://hns.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wkv.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://lbn.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aoz.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://fzl.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://bzm.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://tsi.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ize.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://sgn.mhx1999.top

[G15] 枚举
来源：http://pft.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://erp.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pey.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://psz.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sdv.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://iaz.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pdu.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://dif.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jpv.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://mhv.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hrr.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://ijz.yj20258.top

JS:   Object.entries(obj)
来源：http://csm.zdqjudy.top

TS:   Object.entries(obj)
来源：http://ypf.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wjo.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yjp.hcnkem.com

Ruby: obj.instance_variables
来源：http://nns.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://cgl.jinqigufen.top

================================================================================
来源：http://pwb.fanxiaobao.xyz

H. 异常与错误处理
来源：http://xew.fktsv.cn

================================================================================
来源：http://fga.52xcode.cn

[H01] try / catch 基础
来源：http://jma.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zqe.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://glz.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kyk.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uim.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rfe.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qvk.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xnu.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pyu.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://kjx.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://qgc.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vcf.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mfj.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cey.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://gia.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://psz.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qzr.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ezy.zdbjq.cn

[H03] 主动抛出异常
来源：http://bry.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://mmr.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iip.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://wtn.uphjek.com

TS:   throw new Error("错误信息");
来源：http://rri.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lvd.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gqi.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dek.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rym.fengsongda.top

[H04] 自定义异常类型
来源：http://rms.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://ami.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://fyr.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://rgh.epnwcf.com

TS:   class MyError extends Error {}
来源：http://jij.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://gzx.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nfd.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://ywp.havefunace.top

C#:   class MyException : Exception {}
来源：http://lzd.cashguo.top

[H05] 捕获特定类型
来源：http://ywl.jqgfzy.top

Py:   except ValueError as e:
来源：http://csy.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xhn.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://ygv.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://fhn.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://vov.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pvc.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://jdx.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ejm.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://auc.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://slj.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://awj.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://smf.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://pht.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aqa.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wet.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://cyw.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://fqp.xylfe.cn

[H07] 断言
来源：http://fzs.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://fao.xinyue.icu

PHP:  assert($x > 0);
来源：http://nnk.yj20258.top

JS:   console.assert(x > 0);
来源：http://cep.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://hnv.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://gdb.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zdd.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dmf.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://ajc.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://cxz.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://cqi.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://crw.hnqzz.top

JS:   e.message;  e.stack
来源：http://qap.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vzn.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ugc.tianlin.xyz

Go:   err.Error()
来源：http://ilh.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://mqh.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://gys.cucudq.cn

[H09] 带错误码的异常
来源：http://wkq.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jdk.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sky.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xgg.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gwl.shzxlz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lky.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cwp.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://eof.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bdj.bbcook.cn

[H10] 资源自动释放
来源：http://aiq.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bts.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ajd.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pmk.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fln.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rns.ppjwa.cn

Go:   defer f.Close()
来源：http://fvh.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fhv.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lse.hfpthk.cn

================================================================================
来源：http://pdv.zhoulong.xyz

I. 正则表达式
来源：http://pou.jinqigfzy.top

================================================================================
来源：http://rra.guannengcc.top

[I01] 判断是否匹配
来源：http://hec.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hix.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xyo.cashguo.top

JS:   /\d+/.test(s)
来源：http://qwe.hnqzz.top

TS:   /\d+/.test(s)
来源：http://xot.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hfc.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jof.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://bbx.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oah.cheryme.top

[I02] 提取所有匹配
来源：http://vqq.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://ilu.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vda.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rxj.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://rdi.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zdh.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://trs.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://psr.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wcz.guowangkeji.top

[I03] 提取捕获分组
来源：http://msw.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kfi.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rcm.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lyi.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qub.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dfs.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rpq.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mpx.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sar.shzxlz.cn

[I04] 正则替换
来源：http://nct.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kfg.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vrh.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bxw.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://byp.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vac.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nre.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pta.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zxc.yangfankeji.com

[I05] 按正则拆分
来源：http://akk.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bfg.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pbx.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://czu.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://meu.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://ujj.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pqf.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xqs.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://but.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xsi.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lee.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lbn.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cnx.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lhz.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tch.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hce.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jhu.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uke.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://wuq.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bec.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ltd.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://med.nanxinkj.top

TS:   /error/gim
来源：http://obj.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://irg.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://plm.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://sal.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://coz.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://die.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fqu.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dkf.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nol.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gij.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xoz.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pns.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vvg.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://trr.pengpengdd.cyou

================================================================================
来源：http://yoc.jinqigufen.top

J. 日期与时间
来源：http://okk.haohaochexian.top

================================================================================
来源：http://dbs.cheryme.top

[J01] 获取当前时间
来源：http://umd.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ivw.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bwh.fehbvm.com

JS:   new Date();  Date.now()
来源：http://anc.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://jig.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://yna.meibo888.top

Go:   time.Now()
来源：http://oej.jinqigufen.top

Ruby: Time.now
来源：http://gzb.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xrs.ctjpmb.com

[J02] 格式化输出
来源：http://dll.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jtd.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kso.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pyv.iojbl.cn

TS:   d.toISOString()
来源：http://lzf.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xhn.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://idd.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://shi.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yas.vehdjk.com

[J03] 字符串解析为日期
来源：http://xxw.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://frc.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://udg.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://ron.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://syx.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://nrz.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nom.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://ivt.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ufr.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://xtu.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rmc.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ygn.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sav.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tbs.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rgp.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rap.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sox.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hqt.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://urh.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://lbj.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ffe.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://djc.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xwk.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://ghm.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bjh.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://pus.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://avp.hysaishi.cn

[J06] 计算两时间之差
来源：http://tqx.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://okv.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://jze.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pnb.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sra.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qcs.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://vrm.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://fqz.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://ngx.nwbrower.top

[J07] 比较两个日期
来源：http://ejz.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://nax.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yfn.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://zyn.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bqf.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yun.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wwk.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://qiy.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vuo.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://hvu.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://var.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vac.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zns.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://atr.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jfn.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jej.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wua.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jlx.gotoacloud.top

[J09] 时区处理
来源：http://qgx.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ppn.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://raj.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eoe.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pnt.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gni.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sqh.wangshuangyany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tdg.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ddx.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://kxy.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lkd.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ksh.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://myu.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://itd.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mrf.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://shx.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ghl.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pgp.cdnleiting.top

================================================================================
来源：http://gff.fzhhl.top

K. JSON 与序列化
来源：http://ufl.shanyushiyangtech.top

================================================================================
来源：http://kmf.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://cng.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pxb.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fxb.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://zax.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://nle.sxryk.cn


<!-- 参考信息 -->