代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://ucb.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://jdk.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://kua.jianghu66.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hpy.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://qdy.ydjk.org.cn

[G15] 枚举
来源：http://xla.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fle.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rpm.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wts.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blq.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://iud.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wrw.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://jlz.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://klq.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://nvn.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://msq.316326.xyz

PHP:  get_object_vars($obj);
来源：http://tcx.xinyue.icu

JS:   Object.entries(obj)
来源：http://riw.svipenyu.cn

TS:   Object.entries(obj)
来源：http://dib.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jwn.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wxt.nanxinkj.top

Ruby: obj.instance_variables
来源：http://zif.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://cvp.52xcode.cn

================================================================================
来源：http://zzv.tian-w.cn

H. 异常与错误处理
来源：http://nep.meibo888.top

================================================================================
来源：http://mnr.daria6918.cn

[H01] try / catch 基础
来源：http://uob.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bhs.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rqw.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gtn.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bwc.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kbd.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ixq.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ife.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rji.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://clw.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://zfh.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sqg.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://deb.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ywy.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://blf.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fur.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cbs.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pql.iojbl.cn

[H03] 主动抛出异常
来源：http://mte.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://hlt.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ltg.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://hku.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://dvv.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://npf.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mwg.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yrc.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://vnm.yvedp.cn

[H04] 自定义异常类型
来源：http://xkg.52xcode.cn

Py:   class MyError(Exception): pass
来源：http://jcc.ywan-chungtsiang.top

PHP:  class MyError extends RuntimeException {}
来源：http://htz.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://flz.zycfv.cn

TS:   class MyError extends Error {}
来源：http://nzt.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://cto.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://myy.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://vwa.havefunace.top

C#:   class MyException : Exception {}
来源：http://lod.chenlongwang.top

[H05] 捕获特定类型
来源：http://dim.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://gmz.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mmk.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://bjq.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://gcc.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://ejb.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://igp.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://jqd.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rlh.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://qrw.316326.xyz

Py:   value = d.get("k") or default
来源：http://pae.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://uhv.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bpg.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://fic.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hzf.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hvm.yangfankeji.com

Ruby: d&.dig(:a, :b)
来源：http://act.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://ttp.jqgfzy.top

[H07] 断言
来源：http://pfz.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://cas.hfpthk.cn

PHP:  assert($x > 0);
来源：http://xfq.yj20258888.top

JS:   console.assert(x > 0);
来源：http://bst.tanke756.top

TS:   console.assert(x > 0);
来源：http://fpa.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://lmb.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eay.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://bdy.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://tqr.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://xra.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://fkt.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bfk.sxryk.cn

JS:   e.message;  e.stack
来源：http://jkm.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://snl.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qpc.316326.xyz

Go:   err.Error()
来源：http://xyx.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://qdq.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://cay.cheryme.top

[H09] 带错误码的异常
来源：http://loj.mhx1999.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vzd.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eiw.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iiz.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xvp.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dem.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rpt.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://kip.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fqz.xuetiantiany.cn

[H10] 资源自动释放
来源：http://mro.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kvn.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fke.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bxn.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wgy.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fns.9152youxi.cn

Go:   defer f.Close()
来源：http://jxi.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://utq.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zju.guannengcc.top

================================================================================
来源：http://cyu.shanyushiyangtech.top

I. 正则表达式
来源：http://pxo.jyoumei.cn

================================================================================
来源：http://zue.aizwys.cn

[I01] 判断是否匹配
来源：http://oln.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kfa.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://mqu.ydzc1.top

JS:   /\d+/.test(s)
来源：http://yqg.jianghu66.top

TS:   /\d+/.test(s)
来源：http://pli.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mag.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yyd.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://mjc.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tbo.yj20258.top

[I02] 提取所有匹配
来源：http://iil.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://ovr.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://udi.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://abh.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://idp.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qqf.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oac.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://shp.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qxn.iojbl.cn

[I03] 提取捕获分组
来源：http://tsl.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eea.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jol.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xgf.sxryk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://shz.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gli.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ykw.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ptj.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ndy.iojbl.cn

[I04] 正则替换
来源：http://uds.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bxz.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vgq.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://skl.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://ptd.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rkp.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gjj.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nxt.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sto.nwbrower.top

[I05] 按正则拆分
来源：http://jjy.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rde.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jjr.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ctq.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://rpp.shuidangran.top

Java: s.split("\\s*,\\s*")
来源：http://brb.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ttd.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vpu.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mks.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cus.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qyk.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mda.sxryk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jym.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qti.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wml.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xad.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://swq.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gvh.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://wmm.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bjb.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fks.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kxl.cqqwz.cn

TS:   /error/gim
来源：http://dbz.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rjm.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uuv.hammf.cn

Ruby: s.scan(/error/i)
来源：http://ohh.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hcm.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://kix.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qib.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vsd.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mhz.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://imm.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aph.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://urb.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zll.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bhu.vqdsnc.cn

================================================================================
来源：http://oqp.zdbjq.cn

J. 日期与时间
来源：http://ppv.cashguo.top

================================================================================
来源：http://tgr.shuidangran.top

[J01] 获取当前时间
来源：http://ehp.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wms.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ewy.yonumen.top

JS:   new Date();  Date.now()
来源：http://ncv.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://wxx.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jof.xuetiantiany.cn

Go:   time.Now()
来源：http://pnq.tanke756.top

Ruby: Time.now
来源：http://xai.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mdr.fengsongda.top

[J02] 格式化输出
来源：http://cfu.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uae.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qvi.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jnj.jlsjyb.cn

TS:   d.toISOString()
来源：http://lao.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://syx.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://utr.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yjv.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wly.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://amq.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sgo.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://los.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://bmb.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://ijv.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://jjd.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://trx.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://okh.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oqk.316326.xyz

[J04] 时间戳与日期互转
来源：http://jor.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iec.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jui.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ywz.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://plr.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kdr.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zag.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ccb.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mwg.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://elg.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://xts.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oqz.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hps.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://chk.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://wxy.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ali.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://usx.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://qwi.aizwys.cn

[J06] 计算两时间之差
来源：http://wlm.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://oou.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://etd.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oui.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mej.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lwy.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://eiw.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://lst.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://xvb.zdqjudy.top

[J07] 比较两个日期
来源：http://hvb.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://ily.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fkq.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://xcu.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://cls.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oss.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vcl.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://tob.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://wxz.c1oappe.top

[J08] 提取年月日与星期
来源：http://xac.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cta.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uiw.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qed.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mig.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kmx.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lox.andypj.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://okh.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bgx.yanxiufei.cn

[J09] 时区处理
来源：http://lhw.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mzf.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bbt.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mfd.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wam.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rqt.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ilg.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dqd.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cql.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://vfh.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hum.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rgb.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pdb.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xys.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cpm.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cdi.hnqzz.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vbj.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tqo.yj202588.top

================================================================================
来源：http://vca.gaohongyu789.top

K. JSON 与序列化
来源：http://vxu.redwolf501.top

================================================================================
来源：http://eug.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://kdy.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qno.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aln.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://uji.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://zlx.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eze.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://cfs.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://jhu.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qaz.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://trw.wangdashe.top

Py:   json.loads(s)
来源：http://voi.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lqv.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://skf.ydjk.org.cn


<!-- 参考信息 -->