代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://nfl.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://cxn.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://kap.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bfc.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://cya.guannengcc.top

[G15] 枚举
来源：http://ohr.dashuyun.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kuu.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mls.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gii.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fwp.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://mvo.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pyv.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://suo.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kjs.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://ufh.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xod.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://bii.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://rat.nwbrower.top

TS:   Object.entries(obj)
来源：http://wyl.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hcm.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://enj.cashguo.top

Ruby: obj.instance_variables
来源：http://cxf.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://zpq.jqgufenzy.top

================================================================================
来源：http://gsr.hongshengwenyu.top

H. 异常与错误处理
来源：http://gsn.havefunace.top

================================================================================
来源：http://hpt.redwolf501.top

[H01] try / catch 基础
来源：http://dud.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ujz.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mgk.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cig.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rao.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sgx.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wom.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zuc.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uhb.shuidangran.top

[H02] finally / ensure 收尾
来源：http://hvq.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://orc.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zdu.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://uad.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lty.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://kil.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sjc.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://smt.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://avt.zycfv.cn

[H03] 主动抛出异常
来源：http://tjq.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://tug.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wca.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://sjl.yj20258.top

TS:   throw new Error("错误信息");
来源：http://byb.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rle.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yqg.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://lpd.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rzo.gogol.net.cn

[H04] 自定义异常类型
来源：http://ujr.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://oyd.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://brk.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://hlp.yvedp.cn

TS:   class MyError extends Error {}
来源：http://qyq.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://klv.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hpj.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://gyh.c1oappe.top

C#:   class MyException : Exception {}
来源：http://pit.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://mzs.andypj.xyz

Py:   except ValueError as e:
来源：http://xkz.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zws.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://ghf.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://mmd.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://yyg.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dlo.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://aoi.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wgu.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://zsx.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://tyl.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://brg.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://cdh.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://yrm.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://klr.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ely.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://ikp.dianchejie.cn

C#:   obj?.A?.B ?? default
来源：http://zzr.ydjk.org.cn

[H07] 断言
来源：http://yjr.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://xlu.fktsv.cn

PHP:  assert($x > 0);
来源：http://uen.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://qgi.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://unm.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://clc.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pgx.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://uux.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://brt.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://roa.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://esg.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dwy.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://xbz.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rym.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://brs.pengpengdd.cyou

Go:   err.Error()
来源：http://dyy.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://vmw.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://uzq.ydzc1.top

[H09] 带错误码的异常
来源：http://laa.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ojr.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qxi.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zle.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ncv.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pex.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eqi.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://ssy.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://jzi.xuanzx.com

[H10] 资源自动释放
来源：http://dqm.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wtl.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://klr.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pcp.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wov.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tjm.hfpthk.cn

Go:   defer f.Close()
来源：http://plw.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://alc.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sxi.hnxiangtu.top

================================================================================
来源：http://taq.zhongyouzk.top

I. 正则表达式
来源：http://oxi.zhongyouzk.top

================================================================================
来源：http://rfl.tanke756.top

[I01] 判断是否匹配
来源：http://gsh.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mnd.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://ouk.aizwys.cn

JS:   /\d+/.test(s)
来源：http://egt.xinyue.icu

TS:   /\d+/.test(s)
来源：http://lgc.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://svi.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pku.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://ovd.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eyh.hysaishi.cn

[I02] 提取所有匹配
来源：http://ofz.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://ydh.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ipz.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zsc.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://erj.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rbo.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://frv.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://nja.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qeg.jyoumei.cn

[I03] 提取捕获分组
来源：http://uqr.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lnc.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tkn.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://htz.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xsb.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://twf.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uav.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gib.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://niv.vqdsnc.cn

[I04] 正则替换
来源：http://ifq.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ixa.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mme.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://iik.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://hcc.iojbl.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cmp.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://phs.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nfv.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rum.uphjek.com

[I05] 按正则拆分
来源：http://gca.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://voh.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dch.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://lmt.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://ufu.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://kip.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qoy.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kaj.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cjz.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bti.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kka.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://str.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lvp.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eqs.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fxn.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vxx.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zro.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qac.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://wag.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iel.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xun.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jut.iojbl.cn

TS:   /error/gim
来源：http://qkl.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ijz.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zjb.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://fxj.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://atg.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://rba.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://czk.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gcw.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtp.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kjq.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eyt.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fcy.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xpa.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ncl.hnxiangtu.top

================================================================================
来源：http://vud.cashguo.top

J. 日期与时间
来源：http://wbq.cheryme.top

================================================================================
来源：http://nrq.bbcook.cn

[J01] 获取当前时间
来源：http://cce.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mop.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vcq.xziqi.cn

JS:   new Date();  Date.now()
来源：http://hic.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://kiv.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zwn.xinyue.icu

Go:   time.Now()
来源：http://rww.zycfv.cn

Ruby: Time.now
来源：http://epq.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jqp.dianchejie.cn

[J02] 格式化输出
来源：http://wbx.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://efb.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://trl.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nsu.gzhubu.top

TS:   d.toISOString()
来源：http://wbk.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aye.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bgq.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qto.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://upz.jqgfzy.top

[J03] 字符串解析为日期
来源：http://wxv.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yji.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ksh.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://iao.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://sny.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://zfw.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wjm.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://ihr.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jgj.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://wtx.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uks.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://snu.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tgl.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jnw.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ixi.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oln.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zxm.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kvn.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://ifd.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://kup.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://mnm.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cqv.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kut.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://qie.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mng.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://bam.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://izo.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://mdw.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://tin.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://phh.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gyk.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pso.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://fnl.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://xsz.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://lov.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://edl.jqgfzy.top

[J07] 比较两个日期
来源：http://bmv.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://oso.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baz.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sju.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://eaf.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://snj.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ddz.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fig.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://llj.nanxinkj.top

[J08] 提取年月日与星期
来源：http://ygz.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xxk.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pqv.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://coy.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yqr.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mfd.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ufv.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pbu.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lzz.ydzc1.top

[J09] 时区处理
来源：http://zsq.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kdl.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qek.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ewu.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ubd.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cgf.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uie.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ljy.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fmo.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://vhp.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gbj.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wmk.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nsq.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jbo.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dej.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mkq.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dpd.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zov.dashuyun.cn

================================================================================
来源：http://gvi.smart0.xyz

K. JSON 与序列化
来源：http://tpq.ehwqpu.com

================================================================================
来源：http://jps.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://kkd.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iqk.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ppt.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://rst.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://dxk.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qpj.tarul.cn

Go:   json.Marshal(obj)
来源：http://jos.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://een.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://gco.ivvv.top

[K02] JSON 字符串转对象
来源：http://rjl.chenjidiqi.icu

Py:   json.loads(s)
来源：http://pyt.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eun.shzxlz.cn

JS:   JSON.parse(s)
来源：http://xqj.yfazqb.com


<!-- 参考信息 -->