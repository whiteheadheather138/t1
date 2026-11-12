代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://pkf.birdmap.top

Java: record User(String name, int age) {}
来源：http://zxo.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://fwv.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hxu.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://trv.hfpthk.cn

[G15] 枚举
来源：http://ysw.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://moq.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://scd.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fjz.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vmh.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://ygc.zycfv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ods.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://ehq.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://psv.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://cef.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zvx.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://rte.cheryme.top

JS:   Object.entries(obj)
来源：http://sid.iojbl.cn

TS:   Object.entries(obj)
来源：http://kge.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sgd.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ruw.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://wow.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://shp.yj20258888.top

================================================================================
来源：http://jow.jlsjyb.cn

H. 异常与错误处理
来源：http://ird.cucudq.cn

================================================================================
来源：http://bhb.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://hjb.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://olc.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://roe.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gev.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lck.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://flg.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bcw.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bne.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wzb.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://erh.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://fvf.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yaz.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gtz.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hfy.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://klp.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lyu.zycfv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jvg.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fuh.fktsv.cn

[H03] 主动抛出异常
来源：http://onk.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://ygh.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wvr.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://ryk.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://mqp.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mpw.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uoe.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xlq.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://fwu.hesvh.cn

[H04] 自定义异常类型
来源：http://old.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://ota.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://feh.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://ktj.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://ixo.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://rwi.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://esr.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://udj.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://qit.shzxlz.cn

[H05] 捕获特定类型
来源：http://hfc.wangdashe.top

Py:   except ValueError as e:
来源：http://oib.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://igi.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://fme.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://dep.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://ybx.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://muu.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://jat.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tdw.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://qfz.fzhhl.top

Py:   value = d.get("k") or default
来源：http://chi.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://gbp.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ngy.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://bnh.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nqq.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://aql.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://wpm.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://wyw.cucudq.cn

[H07] 断言
来源：http://cyh.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://tug.sufxvd.cn

PHP:  assert($x > 0);
来源：http://tji.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://rfi.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://dnq.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://abc.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nhj.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://nlq.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://kry.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://rke.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://rxm.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pxm.aizwys.cn

JS:   e.message;  e.stack
来源：http://wzc.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ckt.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mpa.cucudq.cn

Go:   err.Error()
来源：http://pcq.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://ihr.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://ulb.yvedp.cn

[H09] 带错误码的异常
来源：http://scc.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ftg.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jyp.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rci.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://drr.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://awe.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xae.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://dvm.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://eva.yongpay.top

[H10] 资源自动释放
来源：http://gqn.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zuw.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sbh.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fqh.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zrb.yj20258888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://myc.yj202588.top

Go:   defer f.Close()
来源：http://ewr.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://egj.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://plz.yueranfly.top

================================================================================
来源：http://icw.smart0.xyz

I. 正则表达式
来源：http://jcs.chenlongwang.top

================================================================================
来源：http://ndt.ppjwa.cn

[I01] 判断是否匹配
来源：http://ezj.tarul.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mzc.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://khl.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://pfk.tian-w.cn

TS:   /\d+/.test(s)
来源：http://nzp.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gnz.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aaj.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://abu.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vvn.ybcxt.top

[I02] 提取所有匹配
来源：http://gaq.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://bib.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://obu.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eyz.yj202588.top

TS:   s.match(/\d+/g)
来源：http://vio.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sjv.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://icb.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://eec.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wst.tarul.cn

[I03] 提取捕获分组
来源：http://ccx.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ofu.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://czr.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rqj.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ots.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cex.tarul.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cwx.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zoc.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lur.epnwcf.com

[I04] 正则替换
来源：http://ppt.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://enn.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sdc.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://nhy.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://sea.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://pis.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ywq.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ump.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lgv.daria6918.cn

[I05] 按正则拆分
来源：http://yjg.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://phf.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qgo.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://hfz.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://qry.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://iso.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pys.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fmw.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jjs.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tee.andypj.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iho.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://thr.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cku.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hou.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bua.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pik.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fma.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kif.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://rxm.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yut.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yzk.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://egr.smart0.xyz

TS:   /error/gim
来源：http://lmd.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gjy.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://klu.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://hpi.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://exm.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://vxn.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rhq.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://abj.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bby.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://whb.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uqn.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bgz.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://azk.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vin.fanxiaobao.xyz

================================================================================
来源：http://zsq.cdnleiting.top

J. 日期与时间
来源：http://tyw.ydzc1.top

================================================================================
来源：http://aqk.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://ddr.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rhe.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yqf.ivvv.top

JS:   new Date();  Date.now()
来源：http://dhu.yvedp.cn

TS:   new Date();  Date.now()
来源：http://mmn.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mrr.ybcxt.top

Go:   time.Now()
来源：http://knb.svipenyu.cn

Ruby: Time.now
来源：http://xhi.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wra.fengsongda.top

[J02] 格式化输出
来源：http://gwq.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ice.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ins.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hnk.yongpay.top

TS:   d.toISOString()
来源：http://lci.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mpc.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewe.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://glt.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vye.sysykeji.top

[J03] 字符串解析为日期
来源：http://fpj.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mnh.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://buz.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://gag.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://qle.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://orp.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ufm.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://oxz.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vir.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://vuc.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dnz.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iij.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vtw.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xzj.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gfp.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rjm.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://buy.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nxd.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://ban.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://odw.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ejz.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yln.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lap.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://dlx.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jem.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://hnw.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://ayh.ctjpmb.com

[J06] 计算两时间之差
来源：http://nsi.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://cbt.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://qxi.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://chx.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qau.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rat.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://pkj.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://efw.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://udz.ctjpmb.com

[J07] 比较两个日期
来源：http://btb.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://wfv.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yaz.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://opa.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://plo.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xhq.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dbr.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://urw.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://lbk.daxiang520.top

[J08] 提取年月日与星期
来源：http://csy.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fmv.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wor.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fut.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tpl.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wwq.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gss.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ien.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://txx.sjlbkw.cn

[J09] 时区处理
来源：http://pch.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ivs.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yoa.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jbz.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rii.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hgo.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lyv.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://znd.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pvj.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://wxa.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hyy.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xkl.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nxf.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://joy.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pzr.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://itv.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://klg.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://agd.zhaomingkeji.xyz

================================================================================
来源：http://lsj.ivvv.top

K. JSON 与序列化
来源：http://jdt.fanxiaobao.xyz

================================================================================
来源：http://grw.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://jdd.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ozz.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://odt.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://ydc.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://knd.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://snf.hcnkem.com

Go:   json.Marshal(obj)
来源：http://smr.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://cur.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://avi.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://byh.wangdashe.top

Py:   json.loads(s)
来源：http://cnr.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://luy.jyoumei.cn

JS:   JSON.parse(s)
来源：http://ksp.wangshuangyany.cn


<!-- 参考信息 -->