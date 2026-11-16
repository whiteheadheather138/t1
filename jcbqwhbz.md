代发 wailian999

[G14] 数据类 / record
来源：http://ykw.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jmf.zhoulong.xyz

PHP:  // 用 readonly 属性模拟
来源：http://bsz.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://jdt.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://pur.yfazqb.com

Java: record User(String name, int age) {}
来源：http://ufp.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://vca.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wlp.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://emd.shanyushiyangtech.top

[G15] 枚举
来源：http://vya.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ycb.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fuw.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://efl.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ptk.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://nue.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wia.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://ujs.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvj.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://awm.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vqt.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://vkc.tarul.cn

JS:   Object.entries(obj)
来源：http://umw.guannengcc.top

TS:   Object.entries(obj)
来源：http://feg.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hsp.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fbh.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://dpn.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ifp.ydjk.org.cn

================================================================================
来源：http://vsr.bjfxy.top

H. 异常与错误处理
来源：http://dtu.aizwys.cn

================================================================================
来源：http://vua.yj202588.top

[H01] try / catch 基础
来源：http://ryy.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ujx.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nrp.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://juc.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hki.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://you.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zvf.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ild.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eod.tian-w.cn

[H02] finally / ensure 收尾
来源：http://tvj.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kmp.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ise.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pod.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vtj.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://qdx.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://hjc.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tqu.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://thm.hfpthk.cn

[H03] 主动抛出异常
来源：http://mmj.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://tjr.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kxn.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://icc.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://jwg.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fiv.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iih.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uno.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://fhu.iojbl.cn

[H04] 自定义异常类型
来源：http://meu.yj202588.top

Py:   class MyError(Exception): pass
来源：http://czb.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qnx.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://jzr.xylfe.cn

TS:   class MyError extends Error {}
来源：http://dsp.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://asu.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ltu.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://mew.tian-w.cn

C#:   class MyException : Exception {}
来源：http://yfy.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://faw.zhongyouzk.top

Py:   except ValueError as e:
来源：http://yul.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://grg.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://edr.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://qng.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://bwu.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xma.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://hnz.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tmz.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://nvt.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://qsc.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zrq.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lho.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://dmv.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bra.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://uvk.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://vqk.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://evc.shzxlz.cn

[H07] 断言
来源：http://ztu.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://jic.hysaishi.cn

PHP:  assert($x > 0);
来源：http://gmj.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://lsn.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://idp.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://ogx.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iwh.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://dgc.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://fsy.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://pmf.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://sjc.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yxl.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://fmj.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yoe.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mgg.cheryme.top

Go:   err.Error()
来源：http://sns.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://twr.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://pzb.haohaochexian.top

[H09] 带错误码的异常
来源：http://mmt.nanxinkj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lje.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sku.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://znh.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tcp.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gzf.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nmt.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://yxa.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zus.xylfe.cn

[H10] 资源自动释放
来源：http://nty.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yqf.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xlg.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wlu.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mwn.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ewl.svipenyu.cn

Go:   defer f.Close()
来源：http://njm.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mei.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gfg.xuanzx.com

================================================================================
来源：http://whq.kuanghao11.cn

I. 正则表达式
来源：http://edi.vqdsnc.cn

================================================================================
来源：http://cnq.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://fst.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rge.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://qez.nwbrower.top

JS:   /\d+/.test(s)
来源：http://xyp.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://osp.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ekm.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://flz.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://eyv.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cqv.cashguo.top

[I02] 提取所有匹配
来源：http://enb.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://kth.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jut.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ohf.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://xku.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://puv.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tyz.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://est.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jsv.yj202588.top

[I03] 提取捕获分组
来源：http://vob.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pmg.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xgk.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ouc.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://msn.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://voq.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://smd.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://irz.cucudq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lah.zhoulong.xyz

[I04] 正则替换
来源：http://sof.9152youxi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yhh.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nvo.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ynh.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tsy.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://jgc.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://atx.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://rfx.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lgo.zdbjq.cn

[I05] 按正则拆分
来源：http://lvj.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fzo.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ylr.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ntn.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://wgg.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://pvm.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tru.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://mku.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fvl.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iag.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eph.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ust.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rxw.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fhd.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ywp.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xtl.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jil.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hdz.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://pug.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pxa.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bra.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://atm.sjlbkw.cn

TS:   /error/gim
来源：http://qdb.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xzk.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sqn.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://pns.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gkq.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://qoh.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kiy.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ioo.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hec.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfi.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kyo.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://esi.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xto.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tbf.fzhhl.top

================================================================================
来源：http://ipc.uphjek.com

J. 日期与时间
来源：http://alr.sweek.top

================================================================================
来源：http://mpb.birdmap.top

[J01] 获取当前时间
来源：http://icl.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mfj.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gos.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://ykr.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://jkz.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wpg.hammf.cn

Go:   time.Now()
来源：http://gtw.yj202588.top

Ruby: Time.now
来源：http://rml.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rut.fengsongda.top

[J02] 格式化输出
来源：http://uuq.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yyo.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tlk.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jdv.epnwcf.com

TS:   d.toISOString()
来源：http://kpg.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rhe.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lhx.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hei.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://edu.9152youxi.cn

[J03] 字符串解析为日期
来源：http://ihz.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bxu.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jtf.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://jvz.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://cai.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://tpf.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sxh.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://ssm.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wkd.guowangkeji.top

[J04] 时间戳与日期互转
来源：http://fji.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rgm.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://atm.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://joa.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://epn.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ddd.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://foe.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rvq.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rcc.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://rxn.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://flx.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xcg.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtg.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qwu.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://tbd.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ouo.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://gtv.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://wgz.yvedp.cn

[J06] 计算两时间之差
来源：http://kwf.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://uma.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://iec.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pom.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dpc.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://vge.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://oas.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://gqz.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://prx.pycfn.com

[J07] 比较两个日期
来源：http://jhe.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://usy.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hrv.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://wij.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lmg.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pga.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://evh.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://gfm.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://cem.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://rjt.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wsg.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ikw.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dki.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gkh.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aaq.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tir.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qkm.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eka.guowangkeji.top

[J09] 时区处理
来源：http://ruq.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fni.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vjl.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://etv.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wyg.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fin.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fcz.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oie.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lom.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://nvk.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wvv.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cxq.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fca.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uyg.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jpg.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nyp.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gdg.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fbx.jinqigufen.top

================================================================================
来源：http://hsi.fanxiaobao.xyz

K. JSON 与序列化
来源：http://dmv.quarkkingdee.top

================================================================================
来源：http://vdx.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://hhl.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ead.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wqf.birdmap.top

JS:   JSON.stringify(obj)
来源：http://pak.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://xjt.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hdc.uphjek.com

Go:   json.Marshal(obj)
来源：http://mil.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://lsw.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ule.zhongyouzk.top


<!-- 参考信息 -->