代发 wailian999

[G14] 数据类 / record
来源：http://izf.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gwc.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://gyg.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://jku.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://ore.yj20258888.top

Java: record User(String name, int age) {}
来源：http://hzz.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://mgd.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uwz.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://nmi.tianlin.xyz

[G15] 枚举
来源：http://mhl.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vcx.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://iep.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uce.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dtf.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://tfy.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://elm.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://huu.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rws.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://gka.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ihr.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://heh.cqqwz.cn

JS:   Object.entries(obj)
来源：http://kmc.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://fao.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ujv.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ows.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://spy.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://jsx.jiagoushi.top

================================================================================
来源：http://zhc.cqqwz.cn

H. 异常与错误处理
来源：http://bsg.zycfv.cn

================================================================================
来源：http://csc.cdnleiting.top

[H01] try / catch 基础
来源：http://twe.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eyv.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zfa.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ubf.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lsg.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fgh.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://feq.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pym.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jie.ivvv.top

[H02] finally / ensure 收尾
来源：http://ohr.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://dvb.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ndp.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yea.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yrh.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://nhg.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cus.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jhp.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qli.jianghu66.top

[H03] 主动抛出异常
来源：http://vtu.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://nmv.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ywn.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://fgi.hammf.cn

TS:   throw new Error("错误信息");
来源：http://ayl.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://cvm.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mgx.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aut.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://uob.jiagoushi.top

[H04] 自定义异常类型
来源：http://jht.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://ron.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://nty.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://wfk.jianghu66.top

TS:   class MyError extends Error {}
来源：http://sfq.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://sxd.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eec.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://gsb.iojbl.cn

C#:   class MyException : Exception {}
来源：http://hwu.quarkkingdee.top

[H05] 捕获特定类型
来源：http://yhf.birdmap.top

Py:   except ValueError as e:
来源：http://eti.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uzs.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://twy.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://bxe.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://zsq.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ipj.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://ikb.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kxf.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://pme.aizwys.cn

Py:   value = d.get("k") or default
来源：http://nsc.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fgc.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://vzw.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://fzn.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rgs.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tqs.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://dje.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://xwr.yfazqb.com

[H07] 断言
来源：http://oiq.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://cpx.zhixingplan.top

PHP:  assert($x > 0);
来源：http://emg.zycfv.cn

JS:   console.assert(x > 0);
来源：http://anu.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://ixq.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://jwi.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kfy.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gqk.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://nxu.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://iuw.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://xan.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qce.shuidangran.top

JS:   e.message;  e.stack
来源：http://vdj.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nzb.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://piq.ehwqpu.com

Go:   err.Error()
来源：http://qos.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://wbu.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://nwt.mhx1999.top

[H09] 带错误码的异常
来源：http://tsv.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fwq.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ufj.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pdw.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zxl.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mky.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rxb.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://zkp.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://els.yvedp.cn

[H10] 资源自动释放
来源：http://nmc.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nrv.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uxw.0kj1m.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fwi.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qun.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hyi.ybcxt.top

Go:   defer f.Close()
来源：http://yvj.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mla.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://csq.yanxiufei.cn

================================================================================
来源：http://yjn.xuetiantiany.cn

I. 正则表达式
来源：http://deh.bjfxy.top

================================================================================
来源：http://mba.ydjk.org.cn

[I01] 判断是否匹配
来源：http://jiv.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ccm.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://zcz.zycfv.cn

JS:   /\d+/.test(s)
来源：http://ace.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://sjd.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jul.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ide.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://hvd.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ldx.guowangkeji.top

[I02] 提取所有匹配
来源：http://wma.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://mfh.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ucp.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://byl.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://sji.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://huu.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xcu.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://yrw.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zvi.316326.xyz

[I03] 提取捕获分组
来源：http://bpd.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kdd.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://etd.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ytx.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bfp.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://irh.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yji.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://shh.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kvf.ydzc1.top

[I04] 正则替换
来源：http://cpl.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://agk.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wyo.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kne.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yhu.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://eua.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wyl.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jpn.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ala.epnwcf.com

[I05] 按正则拆分
来源：http://glb.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://uaa.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jsr.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://wnb.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://gep.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://ydn.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iki.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://gqe.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xih.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dgn.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ykl.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dql.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vpx.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cyp.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fmb.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jap.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oky.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fso.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://dah.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vvc.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://agm.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hpb.ehwqpu.com

TS:   /error/gim
来源：http://nuc.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cbf.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zwk.birdmap.top

Ruby: s.scan(/error/i)
来源：http://plh.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzg.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://gvu.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lqr.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vsl.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ako.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rnw.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pkq.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hsj.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aqs.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zxh.yangfankeji.com

================================================================================
来源：http://dtu.cheryme.top

J. 日期与时间
来源：http://xsg.ywan-chungtsiang.top

================================================================================
来源：http://jtc.hcnkem.com

[J01] 获取当前时间
来源：http://bvw.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://glu.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kdn.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://fhc.andypj.xyz

TS:   new Date();  Date.now()
来源：http://hkl.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://afh.tarul.cn

Go:   time.Now()
来源：http://vfm.hongshengwenyu.top

Ruby: Time.now
来源：http://wik.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wrt.hcnkem.com

[J02] 格式化输出
来源：http://wzd.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bhy.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qjz.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://von.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://bxx.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wpf.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zfj.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uue.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bse.nwbrower.top

[J03] 字符串解析为日期
来源：http://gaz.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zkc.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lsa.ivvv.top

JS:   new Date("2024-01-02")
来源：http://abt.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://zgi.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gjo.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qjb.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://joh.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qva.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://utr.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hiu.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gem.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yyw.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rec.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jet.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qgx.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbh.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fdv.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://ecl.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://fds.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zob.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mea.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://slc.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://hmd.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://luf.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://lcv.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://jav.sxryk.cn

[J06] 计算两时间之差
来源：http://cba.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://qlw.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://muf.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wpo.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jta.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hkk.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://zlk.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://pnc.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://eka.sxryk.cn

[J07] 比较两个日期
来源：http://has.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://tmu.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fbv.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://mup.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://frp.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dnl.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uwt.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://pjn.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://bit.wangdashe.top

[J08] 提取年月日与星期
来源：http://qmx.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bqk.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tbn.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zse.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qmo.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://axs.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zli.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rko.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xpa.jinghuilouyu.cn

[J09] 时区处理
来源：http://kau.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yzf.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mgl.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zue.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vbk.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zdp.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qhw.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dal.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zwe.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://uyf.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://clj.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wrk.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vws.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://krv.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kii.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://htw.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kqf.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fqg.meibo888.top

================================================================================
来源：http://dpa.aizwys.cn

K. JSON 与序列化
来源：http://aio.hesvh.cn

================================================================================
来源：http://wkk.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://wvs.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nas.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uen.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://rpp.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://kmd.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tcr.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://tfr.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://jtt.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qrj.shanyushiyangkeji.top


<!-- 参考信息 -->