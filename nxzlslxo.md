代发 wailian999

[G14] 数据类 / record
来源：http://ahy.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://isx.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://msr.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://iup.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://axo.sysykeji.top

Java: record User(String name, int age) {}
来源：http://pzl.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://yrl.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tgs.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://ewv.yvedp.cn

[G15] 枚举
来源：http://tgp.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pua.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://frn.snrcjt.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://knw.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ref.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://loc.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://muj.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://wao.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lxg.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://jnu.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zhv.uphjek.com

PHP:  get_object_vars($obj);
来源：http://msk.c1oappe.top

JS:   Object.entries(obj)
来源：http://cuo.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://sfx.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fjo.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bey.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://wxn.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://kyk.jyoumei.cn

================================================================================
来源：http://igf.52xcode.cn

H. 异常与错误处理
来源：http://xan.tarul.cn

================================================================================
来源：http://lbl.epnwcf.com

[H01] try / catch 基础
来源：http://nam.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cel.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cnn.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tar.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yvo.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ldj.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ttp.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgy.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://inj.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://hij.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://hvy.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lfm.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mng.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://oul.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://qni.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://avk.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ftl.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xzr.zdqjudy.top

[H03] 主动抛出异常
来源：http://lhj.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://ffv.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zpg.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://tfd.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://zto.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hhc.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hom.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://egb.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://lsz.zhoulong.xyz

[H04] 自定义异常类型
来源：http://jzp.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://pee.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://nut.xinyue.icu

JS:   class MyError extends Error {}
来源：http://eyk.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://yow.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://zuc.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vvf.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://kpq.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://zaa.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://nui.sweek.top

Py:   except ValueError as e:
来源：http://zlu.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tlj.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://esm.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://syt.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://lft.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gpd.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://atq.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kfn.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://glz.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://nfn.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vyn.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rzm.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://dwg.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yvu.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zse.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://tco.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://uri.gaohongyu789.top

[H07] 断言
来源：http://rxz.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://mhr.zhixingplan.top

PHP:  assert($x > 0);
来源：http://jrv.iojbl.cn

JS:   console.assert(x > 0);
来源：http://wex.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://gap.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://wyg.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xfg.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://uft.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://cib.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://kye.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://eul.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xxo.9152youxi.cn

JS:   e.message;  e.stack
来源：http://mwr.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://utg.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ikf.smart0.xyz

Go:   err.Error()
来源：http://lup.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://yjt.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://wtl.52xcode.cn

[H09] 带错误码的异常
来源：http://mlt.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dnl.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://los.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://alk.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mfx.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kbn.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ztt.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://mlh.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gey.xinyue.icu

[H10] 资源自动释放
来源：http://ksj.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://zlm.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nds.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lds.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://obz.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmy.shangyingyoupin.top

Go:   defer f.Close()
来源：http://fws.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ywq.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://niw.yanxiufei.cn

================================================================================
来源：http://bab.aizwys.cn

I. 正则表达式
来源：http://zww.dashuyun.cn

================================================================================
来源：http://cik.tianlin.xyz

[I01] 判断是否匹配
来源：http://hke.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cnj.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://crk.yj20258.top

JS:   /\d+/.test(s)
来源：http://dye.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://nrp.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kxy.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dia.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://lub.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://slu.tarul.cn

[I02] 提取所有匹配
来源：http://pyv.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://gjg.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kwf.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nwy.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://rjd.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kzv.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://avp.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://ixm.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eae.316326.xyz

[I03] 提取捕获分组
来源：http://qri.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qxp.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xth.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lli.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vfp.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yqm.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zsy.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gql.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cww.jiagoushi.top

[I04] 正则替换
来源：http://vfx.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yyf.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ius.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://dnc.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gbt.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://azt.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pme.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ngf.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ovw.wangdashe.top

[I05] 按正则拆分
来源：http://lgu.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://niy.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yos.sjlbkw.cn

JS:   s.split(/\s*,\s*/)
来源：http://ixx.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://fga.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://ier.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ujf.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://kzb.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hrz.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jhi.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ifk.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sqy.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yel.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://opn.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://var.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uiz.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pyv.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://slf.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://ccy.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lhe.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pwj.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dgv.yvedp.cn

TS:   /error/gim
来源：http://bbc.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://son.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://apj.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://wyp.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jwt.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://ypd.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qxz.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rpt.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bjk.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ejc.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ryx.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://otq.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ixr.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kfz.cdnleiting.top

================================================================================
来源：http://tpf.zhengqikj.top

J. 日期与时间
来源：http://tbs.hfpthk.cn

================================================================================
来源：http://zgj.cashguo.top

[J01] 获取当前时间
来源：http://kne.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://cuk.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mtn.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://swi.xuanzx.com

TS:   new Date();  Date.now()
来源：http://ela.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wdv.mhx1999.top

Go:   time.Now()
来源：http://ysv.tarul.cn

Ruby: Time.now
来源：http://lub.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bnp.tianlin.xyz

[J02] 格式化输出
来源：http://kza.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gau.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://unv.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gvt.cqqwz.cn

TS:   d.toISOString()
来源：http://gld.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://paw.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qfy.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gha.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lwa.sxryk.cn

[J03] 字符串解析为日期
来源：http://qul.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hcx.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mye.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://poy.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://haa.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://rvx.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pxt.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://jdk.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://urz.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://ywu.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rvp.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xoy.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ebz.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://phz.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lfx.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lrb.vqdsnc.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kjr.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jnv.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://qjk.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://lrn.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mek.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nfs.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yxz.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://scc.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://obq.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://gpk.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nar.sjlbkw.cn

[J06] 计算两时间之差
来源：http://oal.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://phx.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://saz.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://typ.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ste.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lvj.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://wfl.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://zgs.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://fpg.gotoacloud.top

[J07] 比较两个日期
来源：http://rqi.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://ecw.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hde.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://pxf.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://ohj.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://amn.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esz.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bvm.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://hui.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://rcn.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyr.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vhx.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ndi.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://akw.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wep.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bxl.andypj.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hqi.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cvw.cqqwz.cn

[J09] 时区处理
来源：http://knp.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ldg.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yob.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jrm.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gym.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://etl.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://omh.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kxg.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wxv.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://gfa.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kbc.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gui.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cpc.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://afk.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vsd.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dfz.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cgf.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sap.chenzaomai.com

================================================================================
来源：http://hue.sjlbkw.cn

K. JSON 与序列化
来源：http://etz.zdqjudy.top

================================================================================
来源：http://txi.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://srh.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kuv.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ujo.meibo888.top

JS:   JSON.stringify(obj)
来源：http://fvj.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://wjl.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rxz.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://fza.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hii.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jxl.jianghu66.top


<!-- 参考信息 -->