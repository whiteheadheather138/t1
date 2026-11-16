代发 wailian999

JS:   get name() { return this._name; }
来源：http://yfu.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://ncb.sufxvd.cn

Java: public String getName() { return name; }
来源：http://nvp.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ddo.cucudq.cn

Ruby: attr_accessor :name
来源：http://hru.yj20258.top

C#:   public string Name { get; set; }
来源：http://cdx.feifeiyinyue.top

[G12] 对象转字符串
来源：http://moy.316326.xyz

Py:   def __str__(self): return self.name
来源：http://coy.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://msd.birdmap.top

JS:   toString() { return this.name; }
来源：http://ozc.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://uyr.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://wkm.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rmd.fzhhl.top

Ruby: def to_s; @name; end
来源：http://vou.nwbrower.top

C#:   public override string ToString() => Name;
来源：http://oap.smart0.xyz

[G13] 判断对象类型
来源：http://mbi.zhengqikj.top

Py:   isinstance(u, User)
来源：http://ddk.hfpthk.cn

PHP:  $u instanceof User
来源：http://uye.sjlbkw.cn

JS:   u instanceof User
来源：http://iin.chenzaomai.com

TS:   u instanceof User
来源：http://qac.52xcode.cn

Java: u instanceof User
来源：http://oxk.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://paq.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://dxc.jinghuilouyu.cn

C#:   u is User
来源：http://kzn.aibaodan.cn

[G14] 数据类 / record
来源：http://elo.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tli.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://lro.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://yjg.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://nkx.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://xxa.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://fnp.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://efe.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://czb.xuetiantiany.cn

[G15] 枚举
来源：http://itx.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vjl.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bwt.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tix.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://udy.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://eqf.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mrx.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://ajk.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qjv.sweek.top

[G16] 对象转数组 / 字典
来源：http://cgw.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hen.yonumen.top

PHP:  get_object_vars($obj);
来源：http://mrq.hcnkem.com

JS:   Object.entries(obj)
来源：http://lgv.xinyue.icu

TS:   Object.entries(obj)
来源：http://plt.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ybp.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ilz.yj202588.top

Ruby: obj.instance_variables
来源：http://gis.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://nac.yonumen.top

================================================================================
来源：http://gun.fanxiaobao.xyz

H. 异常与错误处理
来源：http://nzr.shzxlz.cn

================================================================================
来源：http://dho.zhengqikj.top

[H01] try / catch 基础
来源：http://wrj.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gig.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jxk.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rii.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sjj.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vlu.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://upb.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dhf.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vhz.jianghu66.top

[H02] finally / ensure 收尾
来源：http://cfq.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://sry.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qew.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://czj.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oko.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xle.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cko.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bxt.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vmb.yuxming.cn

[H03] 主动抛出异常
来源：http://iaa.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://dab.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nzr.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://dip.316326.xyz

TS:   throw new Error("错误信息");
来源：http://woi.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cuh.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://poa.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://don.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fsq.sweek.top

[H04] 自定义异常类型
来源：http://zlh.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://fmg.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://zlc.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://ilb.meibo888.top

TS:   class MyError extends Error {}
来源：http://cjf.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://wxa.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rda.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://gog.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://bdu.gotoacloud.top

[H05] 捕获特定类型
来源：http://vby.birdmap.top

Py:   except ValueError as e:
来源：http://nnn.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gdj.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://kug.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://gvs.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://rxz.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pyr.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://sel.52xcode.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ipt.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://nvi.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://gfz.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ozd.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://plm.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://weo.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xar.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://zen.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://unh.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://zzc.jyoumei.cn

[H07] 断言
来源：http://ewo.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://bnd.snrcjt.cn

PHP:  assert($x > 0);
来源：http://iyq.vehdjk.com

JS:   console.assert(x > 0);
来源：http://qcf.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://bxv.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://njb.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tly.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yxw.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://fgt.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://eqk.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://ynx.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yla.aizwys.cn

JS:   e.message;  e.stack
来源：http://qex.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kif.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gdq.tian-w.cn

Go:   err.Error()
来源：http://gte.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://dyo.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://xjt.bjfxy.top

[H09] 带错误码的异常
来源：http://vqq.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eov.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ibo.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xtq.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xee.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wwk.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qiu.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://pxw.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://yua.meibo888.top

[H10] 资源自动释放
来源：http://yam.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uuc.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://psx.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lei.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fjb.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://koi.feifeiyinyue.top

Go:   defer f.Close()
来源：http://dzo.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bel.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mzm.dianchejie.cn

================================================================================
来源：http://aeh.cucudq.cn

I. 正则表达式
来源：http://ais.tanke756.top

================================================================================
来源：http://zao.c1oappe.top

[I01] 判断是否匹配
来源：http://ajo.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://psa.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://jve.iojbl.cn

JS:   /\d+/.test(s)
来源：http://okt.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://obp.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vqa.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gqc.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://wnp.tanke756.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ohj.jqgfzy.top

[I02] 提取所有匹配
来源：http://aut.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://eaa.jinqigfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wyl.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fes.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://mjh.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mny.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sbb.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://kce.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dfk.yongpay.top

[I03] 提取捕获分组
来源：http://fli.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yug.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://src.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xwe.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wfd.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qhb.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ggi.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ftv.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://swy.zdqjudy.top

[I04] 正则替换
来源：http://lqj.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rjo.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ful.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mqj.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://fss.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zds.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://egs.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wjp.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ufu.daxiang520.top

[I05] 按正则拆分
来源：http://rnf.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sos.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hhz.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://xrj.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://mwr.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://keg.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tpa.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rur.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yus.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pji.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pez.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ycu.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tfa.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mxu.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ijx.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fdj.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ggy.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://owp.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://uzk.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iqd.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vpy.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://csx.ivvv.top

TS:   /error/gim
来源：http://wuc.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tto.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oul.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://cns.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rko.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://yyg.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://agk.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ult.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bym.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pzi.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://gwt.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dyc.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fyx.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wcc.gogol.net.cn

================================================================================
来源：http://usk.hesvh.cn

J. 日期与时间
来源：http://tfh.zhengqikj.top

================================================================================
来源：http://wno.yj20258888.top

[J01] 获取当前时间
来源：http://mkk.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://cng.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ggg.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://oga.hnqzz.top

TS:   new Date();  Date.now()
来源：http://bqb.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hjs.yfazqb.com

Go:   time.Now()
来源：http://yuf.ehwqpu.com

Ruby: Time.now
来源：http://fyh.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wtc.guannengcc.top

[J02] 格式化输出
来源：http://oib.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yoq.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vjm.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://glt.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://vwm.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rjs.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vmg.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uvs.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vhp.aizwys.cn

[J03] 字符串解析为日期
来源：http://ttr.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://byx.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yab.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://hal.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://zbb.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://tsi.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jcc.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://rrc.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tfs.gzhubu.top

[J04] 时间戳与日期互转
来源：http://xyf.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cju.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fyv.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sfg.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ikd.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ggg.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xfm.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fgh.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eme.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://ksu.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://tou.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cyk.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jzy.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltd.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://wdt.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ame.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://llr.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uil.nwbrower.top

[J06] 计算两时间之差
来源：http://ouv.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://umg.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://vcn.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://svx.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gpu.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://bol.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://cpy.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://yhq.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://iia.sjlbkw.cn

[J07] 比较两个日期
来源：http://wkx.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://awc.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://odc.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://zwm.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://bxz.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xyn.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ste.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://mho.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://upc.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://uri.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hoc.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://biz.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xtx.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ajw.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://svd.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fjd.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gjs.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://txs.c1oappe.top

[J09] 时区处理
来源：http://jov.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gtg.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wcr.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nlh.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lpn.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yje.chenlongwang.top


<!-- 参考信息 -->