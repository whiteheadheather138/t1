代发 wailian999

Java: u instanceof User
来源：http://fqw.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nzd.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://fqk.shuidangran.top

C#:   u is User
来源：http://mjw.cqqwz.cn

[G14] 数据类 / record
来源：http://zvw.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lyg.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://mma.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kvn.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://jkj.uphjek.com

Java: record User(String name, int age) {}
来源：http://tju.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://keh.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rcf.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://nha.epnwcf.com

[G15] 枚举
来源：http://ase.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zli.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsq.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://msd.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cej.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://csv.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hfy.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://ydx.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ccu.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://vqz.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wfp.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://xyi.cdnleiting.top

JS:   Object.entries(obj)
来源：http://pmr.0kj1m.cn

TS:   Object.entries(obj)
来源：http://ghp.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mul.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qgl.316326.xyz

Ruby: obj.instance_variables
来源：http://qqj.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://bkd.bjfxy.top

================================================================================
来源：http://jci.aizwys.cn

H. 异常与错误处理
来源：http://ver.tarul.cn

================================================================================
来源：http://kns.cqqwz.cn

[H01] try / catch 基础
来源：http://pyu.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bre.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xxh.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tqv.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://csc.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qpb.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bfh.ehwqpu.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wbh.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ycf.hnqzz.top

[H02] finally / ensure 收尾
来源：http://opd.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wdk.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qlc.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://old.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xfl.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://yob.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tmp.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mav.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://bja.vehdjk.com

[H03] 主动抛出异常
来源：http://qxn.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://koe.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hkc.havefunace.top

JS:   throw new Error("错误信息");
来源：http://dbi.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://rki.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pxf.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zjp.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cah.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://xkq.gzhubu.top

[H04] 自定义异常类型
来源：http://cjs.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://ipy.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bam.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://wke.fanxiaobao.xyz

TS:   class MyError extends Error {}
来源：http://swi.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://fzk.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tak.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://rbh.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://cdj.ybcxt.top

[H05] 捕获特定类型
来源：http://toi.aibaodan.cn

Py:   except ValueError as e:
来源：http://cbe.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xkt.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://xsj.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://ibv.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://tao.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lys.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://tcr.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qqk.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://eny.vehdjk.com

Py:   value = d.get("k") or default
来源：http://pya.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://ejx.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hfx.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ede.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mbs.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://obc.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://lgr.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://vub.yonumen.top

[H07] 断言
来源：http://vyn.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://eau.tanke756.top

PHP:  assert($x > 0);
来源：http://psb.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://efp.yj20258.top

TS:   console.assert(x > 0);
来源：http://pec.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://zul.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jvz.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sxs.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://riy.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://gys.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://hdi.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vvq.316326.xyz

JS:   e.message;  e.stack
来源：http://xvo.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fjr.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iht.fengsongda.top

Go:   err.Error()
来源：http://zea.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://pdr.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://ilr.hysaishi.cn

[H09] 带错误码的异常
来源：http://rgs.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dks.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nzk.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dns.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xqe.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ynk.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://due.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sty.ywan-chungtsiang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://grd.wangdashe.top

[H10] 资源自动释放
来源：http://dfg.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wlg.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xkc.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qrf.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wfj.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hxe.gotoacloud.top

Go:   defer f.Close()
来源：http://btn.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yrw.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gci.xuanzx.com

================================================================================
来源：http://mtf.jinqigfzy.top

I. 正则表达式
来源：http://ytf.nanxuanxn.top

================================================================================
来源：http://nwr.ydjk.org.cn

[I01] 判断是否匹配
来源：http://stc.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dlm.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://srz.uphjek.com

JS:   /\d+/.test(s)
来源：http://cwx.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://fdy.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lvh.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dng.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://msj.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qim.uphjek.com

[I02] 提取所有匹配
来源：http://amr.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://gub.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vxu.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gem.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://fgz.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tle.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gxr.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://pst.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vnj.cdnleiting.top

[I03] 提取捕获分组
来源：http://ffd.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kcf.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gnx.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://unk.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://olt.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gja.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ybh.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cge.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://irt.ehwqpu.com

[I04] 正则替换
来源：http://bso.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xam.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vma.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cbo.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ibd.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://dwp.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gvk.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zrb.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lle.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://jfw.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://dpj.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qau.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://pni.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://xlh.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://pet.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gin.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://eeg.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://isi.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rqz.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bfz.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kjc.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fzf.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vzi.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ykd.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ybw.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gna.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://stz.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://zms.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://stv.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kxh.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jnk.shangyingyoupin.top

TS:   /error/gim
来源：http://mah.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://big.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ldl.hammf.cn

Ruby: s.scan(/error/i)
来源：http://jiy.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fjw.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://key.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tjg.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yjr.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ntx.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nwy.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zxv.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vbn.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://peu.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vqr.cashguo.top

================================================================================
来源：http://sxz.daria6918.cn

J. 日期与时间
来源：http://qsa.sweek.top

================================================================================
来源：http://ixf.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://pzc.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fmf.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sth.fzhhl.top

JS:   new Date();  Date.now()
来源：http://bbg.sysykeji.top

TS:   new Date();  Date.now()
来源：http://brn.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wev.shuidangran.top

Go:   time.Now()
来源：http://uuh.chenlongwang.top

Ruby: Time.now
来源：http://kdx.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ucd.epnwcf.com

[J02] 格式化输出
来源：http://vdu.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jxz.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wld.pycfn.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ute.smart0.xyz

TS:   d.toISOString()
来源：http://vec.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xpj.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://san.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jdn.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pug.fktsv.cn

[J03] 字符串解析为日期
来源：http://wzc.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rid.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dyb.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://wfv.yonumen.top

TS:   new Date("2024-01-02")
来源：http://wda.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://utt.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yqe.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://hbk.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pxa.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://qly.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bye.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qmy.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://clp.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qug.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://svs.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zaf.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nod.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oxv.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://rvf.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://dvn.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cxy.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://znk.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jge.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://yij.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://izo.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://zvo.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://geb.yj202588.top

[J06] 计算两时间之差
来源：http://ugo.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://gok.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://etp.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sfc.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ezr.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bfz.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://coc.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://kwr.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://uyz.cashguo.top

[J07] 比较两个日期
来源：http://jjs.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://mop.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dkg.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://irv.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://oxw.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tlq.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gut.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://pgu.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://iow.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://ttb.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jjg.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cgy.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jys.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jii.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cno.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wxz.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ztv.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dkw.sjlbkw.cn

[J09] 时区处理
来源：http://nzu.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://apu.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agi.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://euc.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qun.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xnn.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tjh.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fbm.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://swo.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://xiz.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://rnh.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sxs.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tfz.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qdh.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sjz.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jdl.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ioc.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://scm.aibaodan.cn

================================================================================
来源：http://zes.ppjwa.cn

K. JSON 与序列化
来源：http://oyj.sufxvd.cn

================================================================================
来源：http://ifw.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://btx.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rli.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fgr.cdnleiting.top

JS:   JSON.stringify(obj)
来源：http://kew.316326.xyz

TS:   JSON.stringify(obj)
来源：http://vkf.gotoacloud.top


<!-- 参考信息 -->