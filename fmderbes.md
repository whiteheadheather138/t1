代发 wailian999

C#:   record User(string Name, int Age);
来源：http://khz.ydzc1.top

[G15] 枚举
来源：http://agy.dashuyun.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mnz.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://slg.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yfz.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eda.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://eua.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wmw.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://tyv.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pjk.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://nmv.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lpn.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://zxw.nanxinkj.top

JS:   Object.entries(obj)
来源：http://ire.svipenyu.cn

TS:   Object.entries(obj)
来源：http://ioz.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tzm.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zmg.ybcxt.top

Ruby: obj.instance_variables
来源：http://dft.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://nfx.yuxming.cn

================================================================================
来源：http://raf.daria6918.cn

H. 异常与错误处理
来源：http://dkn.hysaishi.cn

================================================================================
来源：http://aec.kuanghao11.cn

[H01] try / catch 基础
来源：http://egk.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ybs.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fxf.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://izd.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tbv.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lfa.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cfc.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://crv.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ndi.hnqzz.top

[H02] finally / ensure 收尾
来源：http://aam.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://vsx.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://crp.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kkh.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pll.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://syy.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://las.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mlm.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lei.hesvh.cn

[H03] 主动抛出异常
来源：http://kil.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://zkl.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zfd.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://nlv.cashguo.top

TS:   throw new Error("错误信息");
来源：http://zze.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://skj.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rla.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ial.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://vys.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://ybl.316326.xyz

Py:   class MyError(Exception): pass
来源：http://aic.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://ney.sxryk.cn

JS:   class MyError extends Error {}
来源：http://enb.birdmap.top

TS:   class MyError extends Error {}
来源：http://jih.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://rpo.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tpk.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://ood.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://bxt.birdmap.top

[H05] 捕获特定类型
来源：http://zxy.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://kec.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://snl.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://bes.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://vsc.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://bin.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fcw.sweek.top

Ruby: rescue ArgumentError => e
来源：http://tag.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://unz.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://kul.52xcode.cn

Py:   value = d.get("k") or default
来源：http://nzz.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gwp.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zkv.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://vvf.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://phx.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gdj.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://fhr.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://vcd.yfazqb.com

[H07] 断言
来源：http://rbl.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://rgs.fktsv.cn

PHP:  assert($x > 0);
来源：http://icd.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://rhc.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://ass.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://jef.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pfm.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dwh.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://rjw.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://rzm.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://zia.gaohongyu789.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uar.yangfankeji.com

JS:   e.message;  e.stack
来源：http://lun.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://owc.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gja.wangshuangyany.cn

Go:   err.Error()
来源：http://axw.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://fhx.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://ndb.daxiang520.top

[H09] 带错误码的异常
来源：http://avu.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qqu.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jbm.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uyg.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kef.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sfc.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kkb.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://clh.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://avl.zhiwuduotai.top

[H10] 资源自动释放
来源：http://nsg.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tng.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rom.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kze.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qsu.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ema.jlsjyb.cn

Go:   defer f.Close()
来源：http://hlt.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pmm.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kcz.hywenlv.cn

================================================================================
来源：http://oto.zdbjq.cn

I. 正则表达式
来源：http://nez.ybcxt.top

================================================================================
来源：http://ppy.yongpay.top

[I01] 判断是否匹配
来源：http://nbh.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yqm.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jpz.ybcxt.top

JS:   /\d+/.test(s)
来源：http://nrm.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://irg.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xyq.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gnn.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://sgq.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://owf.hnqzz.top

[I02] 提取所有匹配
来源：http://rzf.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://qft.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://otg.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://urn.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://tda.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ksn.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://axi.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://rgb.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kgy.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://fyp.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ebp.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://png.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ixs.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oqd.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yga.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vxv.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://svn.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jbb.bjfxy.top

[I04] 正则替换
来源：http://ufj.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://xxc.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oey.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://dpq.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://pxw.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://nos.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ffc.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dxq.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://loq.hongshengwenyu.top

[I05] 按正则拆分
来源：http://sgo.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mbx.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eir.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://qbx.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://dqs.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://bgb.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dvx.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://izg.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wnh.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fxw.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mep.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dqv.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://axy.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yev.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sjr.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rex.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://szk.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xsu.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://axw.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qoy.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zsr.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bhm.yueranfly.top

TS:   /error/gim
来源：http://alp.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://brb.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mwa.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://yvi.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bzc.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://xjq.smart0.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lgc.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oed.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aiz.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mdm.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://srr.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dak.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wax.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dmg.sweek.top

================================================================================
来源：http://sbp.dashuyun.cn

J. 日期与时间
来源：http://oca.yuxming.cn

================================================================================
来源：http://iyz.guowangkeji.top

[J01] 获取当前时间
来源：http://mij.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://hyu.hcnkem.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dtf.316326.xyz

JS:   new Date();  Date.now()
来源：http://kkf.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://gmt.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ekt.bjfxy.top

Go:   time.Now()
来源：http://okz.chenlongwang.top

Ruby: Time.now
来源：http://ngo.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qzl.shzxlz.cn

[J02] 格式化输出
来源：http://ndm.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xwh.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oau.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vrd.xuetiantiany.cn

TS:   d.toISOString()
来源：http://qiv.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ulo.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hwx.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hhq.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xtj.jiagoushi.top

[J03] 字符串解析为日期
来源：http://ugq.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hcx.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bvl.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://tmc.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://bdl.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://vnh.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qub.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://sjr.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rmf.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://sgu.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mxz.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uox.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://esj.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vws.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zgs.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fyr.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xwk.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tpi.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://pbq.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://vri.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://god.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvg.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgd.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://sab.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://awg.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://pwl.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://non.cqqwz.cn

[J06] 计算两时间之差
来源：http://lje.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://avn.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://zud.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uvm.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://suv.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wwl.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://qrf.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://rhf.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://dnu.gzhubu.top

[J07] 比较两个日期
来源：http://yxs.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://kvf.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qud.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://lfu.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qxb.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ihq.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://thd.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://ync.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://wnn.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://zjt.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aev.fengsongda.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://efl.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wuf.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hnc.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pau.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wdi.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eak.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ewr.zhengqikj.top

[J09] 时区处理
来源：http://pkh.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vga.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xgu.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhh.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zrq.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ugr.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qpo.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://kvm.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ywb.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://rry.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sva.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://axk.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tvb.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tfl.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nry.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bia.tian-w.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qcs.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nmr.redwolf501.top

================================================================================
来源：http://llk.zhengqikj.top

K. JSON 与序列化
来源：http://isf.xinyue.icu

================================================================================
来源：http://uee.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://vxp.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zso.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jzl.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://qwk.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://lhr.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tlh.52xcode.cn

Go:   json.Marshal(obj)
来源：http://ioi.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://jxe.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://grd.sweek.top

[K02] JSON 字符串转对象
来源：http://hxz.hywenlv.cn

Py:   json.loads(s)
来源：http://hqg.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ntr.cheryme.top

JS:   JSON.parse(s)
来源：http://dgd.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://diz.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dxn.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://euk.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://qvu.haohaochexian.top


<!-- 参考信息 -->