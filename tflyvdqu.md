代发 wailian999

[G14] 数据类 / record
来源：http://brs.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nte.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://qqx.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kzc.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://wsb.fehbvm.com

Java: record User(String name, int age) {}
来源：http://vmr.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://sab.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bsz.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://mqh.xingfuxueyuan.xyz

[G15] 枚举
来源：http://nnm.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hpb.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ajk.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ydr.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sgc.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://ljf.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ico.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://ilm.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://amb.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://fjb.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rqt.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://uct.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://efa.fktsv.cn

TS:   Object.entries(obj)
来源：http://jml.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bce.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://grr.hesvh.cn

Ruby: obj.instance_variables
来源：http://for.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://hlq.hnqzz.top

================================================================================
来源：http://iet.jiagoushi.top

H. 异常与错误处理
来源：http://lep.c1oappe.top

================================================================================
来源：http://sqc.jinqigufen.top

[H01] try / catch 基础
来源：http://bwg.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eah.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zbn.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ork.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ffi.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://row.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fle.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sht.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jzu.smart0.xyz

[H02] finally / ensure 收尾
来源：http://nzo.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://fki.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cwd.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mdp.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://eid.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://ofa.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://mzq.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bdg.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jwy.gzhubu.top

[H03] 主动抛出异常
来源：http://siy.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://vfr.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://apa.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://rer.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://qfg.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xls.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mvs.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xwi.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://rnd.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://cie.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://zyl.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://ejn.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://qjs.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://lol.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://btv.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://opf.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://kyv.daxiang520.top

C#:   class MyException : Exception {}
来源：http://ang.ydjk.org.cn

[H05] 捕获特定类型
来源：http://fos.gogol.net.cn

Py:   except ValueError as e:
来源：http://fud.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yka.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://omj.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://hpl.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://cki.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qek.yuxming.cn

Ruby: rescue ArgumentError => e
来源：http://jwd.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rqq.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://vpy.tian-w.cn

Py:   value = d.get("k") or default
来源：http://avp.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://lat.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://odw.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://sdb.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ukl.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yoy.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://ova.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://kqv.snrcjt.cn

[H07] 断言
来源：http://sew.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://gsu.gotoacloud.top

PHP:  assert($x > 0);
来源：http://elb.tarul.cn

JS:   console.assert(x > 0);
来源：http://ruz.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://auk.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://hva.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lzm.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://jph.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://wny.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://sqj.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://iwf.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mqx.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://aac.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kmy.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yul.quarkkingdee.top

Go:   err.Error()
来源：http://uwh.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://jtq.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://btk.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://iqs.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lbg.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ybx.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gpi.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mtl.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bhe.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ice.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://yfe.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://lpj.52xcode.cn

[H10] 资源自动释放
来源：http://fol.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://iln.yueranfly.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ogi.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyy.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://veh.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://giy.c1oappe.top

Go:   defer f.Close()
来源：http://dxc.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gtn.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://abz.ehwqpu.com

================================================================================
来源：http://fuc.hnxiangtu.top

I. 正则表达式
来源：http://eqa.guannengcc.top

================================================================================
来源：http://wgc.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://jzc.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fyl.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://rsa.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://vih.fehbvm.com

TS:   /\d+/.test(s)
来源：http://fcv.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://omx.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fjk.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://pnj.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lbm.sufxvd.cn

[I02] 提取所有匹配
来源：http://kpa.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://ksl.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bah.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tgp.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://hha.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blt.xylfe.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gay.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://uyc.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ybl.ehwqpu.com

[I03] 提取捕获分组
来源：http://fcq.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qbx.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nea.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fef.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hzq.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hnm.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nsu.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wkd.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wdo.chenjidiqi.icu

[I04] 正则替换
来源：http://frp.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://xki.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ilz.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://joo.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://qnj.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://gjs.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xtw.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://wfw.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://abd.xuetiantiany.cn

[I05] 按正则拆分
来源：http://uww.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://bbh.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ofl.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://zuj.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://xok.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://let.dianchejie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://loi.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://xoc.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xlw.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fnt.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qjs.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nhm.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qpt.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dor.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zne.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bry.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cwk.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mlf.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://rgh.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ait.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yew.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://izi.ywan-chungtsiang.top

TS:   /error/gim
来源：http://dlc.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ste.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://toe.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://dgu.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yej.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://vkv.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cmu.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cym.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iin.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sqf.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bhp.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cdi.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gfn.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qsa.feifeiyinyue.top

================================================================================
来源：http://prk.sweek.top

J. 日期与时间
来源：http://doz.ehwqpu.com

================================================================================
来源：http://uef.yuanzhike.top

[J01] 获取当前时间
来源：http://sga.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hmq.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xgf.fzhhl.top

JS:   new Date();  Date.now()
来源：http://ffq.sxryk.cn

TS:   new Date();  Date.now()
来源：http://xte.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jjd.jlsjyb.cn

Go:   time.Now()
来源：http://ssu.jinqigufen.top

Ruby: Time.now
来源：http://qmz.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yek.gzhubu.top

[J02] 格式化输出
来源：http://aoj.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://swe.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://izx.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ruo.feifeiyinyue.top

TS:   d.toISOString()
来源：http://iri.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://udo.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zxn.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qrk.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jkp.hysaishi.cn

[J03] 字符串解析为日期
来源：http://qic.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fwl.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://taa.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://jss.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://opb.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://dmo.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oaw.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://mcu.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aja.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://sxn.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cka.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yvp.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://esa.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ilu.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cin.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://won.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bso.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://waz.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://qeq.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://qxo.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mll.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mhi.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://axt.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://vsw.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sqp.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://vhy.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://pjs.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://vms.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://ejf.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://hvv.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sid.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lee.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://dwd.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://xkf.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://yri.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://aex.hnxiangtu.top

[J07] 比较两个日期
来源：http://bfe.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://zto.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qjb.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://mhp.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://xgu.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://byu.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jjj.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hms.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://gqy.zdqjudy.top

[J08] 提取年月日与星期
来源：http://plq.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ygn.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cdy.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hvb.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kkl.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eii.hywenlv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pab.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tgh.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iwx.haohaochexian.top

[J09] 时区处理
来源：http://baw.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nqd.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rfh.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://noz.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dbw.snrcjt.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hwk.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sab.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fhz.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cuu.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://yqm.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://luu.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://upi.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yet.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zko.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xsn.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://phq.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uit.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tuw.cheryme.top

================================================================================
来源：http://jax.xuetiantiany.cn

K. JSON 与序列化
来源：http://nqc.hammf.cn

================================================================================
来源：http://bkd.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://olr.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kbj.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zzb.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://nrs.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://mms.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wbu.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://hww.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://dmn.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xau.zdqjudy.top


<!-- 参考信息 -->