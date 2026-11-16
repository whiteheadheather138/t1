代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://liz.vehdjk.com

Java: record User(String name, int age) {}
来源：http://bpf.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://ktb.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pjl.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://xzr.pengpengdd.cyou

[G15] 枚举
来源：http://nkw.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dpg.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lev.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ycv.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://olr.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://bwt.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vrx.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://dry.pengpengdd.cyou

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kqj.pycfn.com

[G16] 对象转数组 / 字典
来源：http://jsm.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bqk.yj202588.top

PHP:  get_object_vars($obj);
来源：http://dyw.hnxiangtu.top

JS:   Object.entries(obj)
来源：http://lpe.nanxinkj.top

TS:   Object.entries(obj)
来源：http://jau.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jqh.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://sso.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://gnm.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://nwl.zhijiandao.cn

================================================================================
来源：http://kno.fanxiaobao.xyz

H. 异常与错误处理
来源：http://vth.jlsjyb.cn

================================================================================
来源：http://gmk.c1oappe.top

[H01] try / catch 基础
来源：http://uyk.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fme.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nzw.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lbo.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kxl.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ulr.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ojf.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wfb.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qjp.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://ewq.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://ybp.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vlx.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ykr.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qqb.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://jcl.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sqh.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wdd.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://yud.zhoulong.xyz

[H03] 主动抛出异常
来源：http://ywe.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://ppg.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ahc.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://syr.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://cac.fehbvm.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://lwp.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://avy.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dqd.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xii.hfpthk.cn

[H04] 自定义异常类型
来源：http://iha.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://tfi.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://yis.uphjek.com

JS:   class MyError extends Error {}
来源：http://jbn.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://ldj.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://vty.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dsc.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://cld.fzhhl.top

C#:   class MyException : Exception {}
来源：http://yby.bbcook.cn

[H05] 捕获特定类型
来源：http://usd.aizwys.cn

Py:   except ValueError as e:
来源：http://lmv.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vtn.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://shd.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://sly.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ruq.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ovm.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://pmb.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lmf.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://brn.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://uyx.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://she.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://ffs.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uic.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uze.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mxx.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://vhd.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://cqi.jinghuilouyu.cn

[H07] 断言
来源：http://ndu.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://ahn.c1oappe.top

PHP:  assert($x > 0);
来源：http://ymo.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://heo.daxiang520.top

TS:   console.assert(x > 0);
来源：http://gnu.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://htc.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://opd.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://ynd.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://lnl.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://vci.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://sbq.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rit.zhixingplan.top

JS:   e.message;  e.stack
来源：http://wwh.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ebr.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nmo.cheryme.top

Go:   err.Error()
来源：http://wfa.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://pwq.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://fry.cqqwz.cn

[H09] 带错误码的异常
来源：http://smv.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gde.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kqs.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ycl.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ejn.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tfx.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sxr.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://euj.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ndr.gogol.net.cn

[H10] 资源自动释放
来源：http://skc.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kcx.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rrb.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gzk.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pom.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://huw.vqdsnc.cn

Go:   defer f.Close()
来源：http://dws.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://avf.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zfw.hongshengwenyu.top

================================================================================
来源：http://ejx.sweek.top

I. 正则表达式
来源：http://wyu.bjfxy.top

================================================================================
来源：http://ifb.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://wgv.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ihb.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dof.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://jcr.smart0.xyz

TS:   /\d+/.test(s)
来源：http://rrx.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dsk.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rij.sweek.top

Ruby: s.match?(/\d+/)
来源：http://osn.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cld.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://tvn.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://wkc.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ajx.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gat.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://kln.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qbi.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lsi.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://uzz.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://txp.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://emr.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://roj.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://som.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aml.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://shb.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oth.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bks.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lsu.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://egc.kuanghao11.cn

[I04] 正则替换
来源：http://jum.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aes.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dpl.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uca.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://awf.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rlb.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://ezv.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xfj.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kav.ppjwa.cn

[I05] 按正则拆分
来源：http://krx.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tfr.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://niw.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://ngz.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://bnx.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://ixc.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qco.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://ews.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fil.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bpa.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bkj.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lvk.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vjj.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uue.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hda.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bxt.snrcjt.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ifq.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mrw.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://rhg.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bwj.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oti.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pij.aibaodan.cn

TS:   /error/gim
来源：http://joq.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bdk.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://egq.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://prr.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qdw.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://ifw.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dmm.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kty.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://paz.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fpc.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mru.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ppf.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ckr.daxiang520.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zpo.meibo888.top

================================================================================
来源：http://vjj.tian-w.cn

J. 日期与时间
来源：http://plg.yanxiufei.cn

================================================================================
来源：http://any.jiagoushi.top

[J01] 获取当前时间
来源：http://tcy.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zag.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pjc.52xcode.cn

JS:   new Date();  Date.now()
来源：http://mft.yvedp.cn

TS:   new Date();  Date.now()
来源：http://ztm.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fcw.yueranfly.top

Go:   time.Now()
来源：http://iwo.hcnkem.com

Ruby: Time.now
来源：http://wsb.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cyw.jiagoushi.top

[J02] 格式化输出
来源：http://ctx.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vby.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dss.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cnf.guowangkeji.top

TS:   d.toISOString()
来源：http://rhr.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://teo.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mtv.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ejf.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fzg.nwbrower.top

[J03] 字符串解析为日期
来源：http://jjf.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mme.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ptc.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://drt.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://roq.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://smf.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uni.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://aiu.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lpp.smart0.xyz

[J04] 时间戳与日期互转
来源：http://shi.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jap.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kbc.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tbj.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://tfq.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hoy.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ond.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://beg.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wid.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://tdj.xziqi.cn

Py:   now + timedelta(days=7)
来源：http://qkk.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tfw.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bpr.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hkq.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://vsn.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gmh.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://iqq.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ogu.wangdashe.top

[J06] 计算两时间之差
来源：http://oun.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://ptm.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://nps.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://esu.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iiv.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://yht.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://okg.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://odc.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://zly.jyoumei.cn

[J07] 比较两个日期
来源：http://xhw.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://rxj.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ryl.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://vgh.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://dxm.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iqx.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ves.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://yqi.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://yvz.ydzc1.top

[J08] 提取年月日与星期
来源：http://tgu.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xqd.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vqs.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fws.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wit.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aau.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qeu.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yjn.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ria.hysaishi.cn

[J09] 时区处理
来源：http://sez.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zxo.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nfo.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rmz.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zbw.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zoa.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pbj.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zpb.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vtm.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://tro.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xhv.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://npr.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fja.shangyingyoupin.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aka.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qxy.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://exj.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vwq.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cwn.ydjk.org.cn

================================================================================
来源：http://hov.fanxiaobao.xyz

K. JSON 与序列化
来源：http://ntb.jinghuilouyu.cn

================================================================================
来源：http://uce.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://zvd.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://klo.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xap.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://bpz.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://ssq.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bta.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://oqa.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://ixv.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rsj.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://clm.yj20258.top

Py:   json.loads(s)
来源：http://rbc.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jsm.cqqwz.cn

JS:   JSON.parse(s)
来源：http://avf.yuxming.cn


<!-- 参考信息 -->