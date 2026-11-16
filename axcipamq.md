代发 wailian999

C#:   public / protected / private / internal
来源：http://gsz.hongshengwenyu.top

[G11] getter / setter
来源：http://bwf.fktsv.cn

Py:   @property 与 @x.setter
来源：http://kim.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tft.sxryk.cn

JS:   get name() { return this._name; }
来源：http://dwi.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://yjc.dashuyun.cn

Java: public String getName() { return name; }
来源：http://dik.hammf.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://moy.hammf.cn

Ruby: attr_accessor :name
来源：http://ghm.cucudq.cn

C#:   public string Name { get; set; }
来源：http://sxd.hysaishi.cn

[G12] 对象转字符串
来源：http://kxl.tanke756.top

Py:   def __str__(self): return self.name
来源：http://fdr.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cpu.aizwys.cn

JS:   toString() { return this.name; }
来源：http://wcs.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://wmi.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://pgx.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://djq.tarul.cn

Ruby: def to_s; @name; end
来源：http://ykp.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://nhz.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://asw.yonumen.top

Py:   isinstance(u, User)
来源：http://fwl.snrcjt.cn

PHP:  $u instanceof User
来源：http://blm.aibaodan.cn

JS:   u instanceof User
来源：http://kzt.epnwcf.com

TS:   u instanceof User
来源：http://rpg.yuanzhike.top

Java: u instanceof User
来源：http://bez.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://yoq.yvedp.cn

Ruby: u.is_a?(User)
来源：http://gzw.wangshuangyany.cn

C#:   u is User
来源：http://abu.yj20258888.top

[G14] 数据类 / record
来源：http://wku.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dze.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://ofc.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://ruo.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://nwn.tanke756.top

Java: record User(String name, int age) {}
来源：http://qhx.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://axr.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bqq.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://ell.yuanzhike.top

[G15] 枚举
来源：http://lhi.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://twz.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mhv.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tsb.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qff.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://xpg.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fyj.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://iwj.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pyl.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://txh.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://npi.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://vsx.yuxming.cn

JS:   Object.entries(obj)
来源：http://rgs.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://rjt.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qnc.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zcr.iojbl.cn

Ruby: obj.instance_variables
来源：http://rnx.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://jvd.cqqwz.cn

================================================================================
来源：http://djz.xuetiantiany.cn

H. 异常与错误处理
来源：http://wsb.hcnkem.com

================================================================================
来源：http://tye.316326.xyz

[H01] try / catch 基础
来源：http://ari.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lnh.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lkk.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mcc.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fgd.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vms.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wwe.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fmk.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://koe.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://xvo.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hbl.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bsv.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://zxg.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://btz.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mir.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lev.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://akc.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lzv.jinqigfzy.top

[H03] 主动抛出异常
来源：http://efu.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://cwk.vqdsnc.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bww.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://gqv.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://bfy.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uip.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ieu.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://spz.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://siq.c1oappe.top

[H04] 自定义异常类型
来源：http://qep.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://gxy.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://zls.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://hmm.bbcook.cn

TS:   class MyError extends Error {}
来源：http://rwu.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://tgk.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uen.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://orr.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://zfq.ehwqpu.com

[H05] 捕获特定类型
来源：http://kbj.quarkkingdee.top

Py:   except ValueError as e:
来源：http://ppj.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qjh.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://uas.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://ths.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://lkq.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lif.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://yxr.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dct.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://qnp.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://bpc.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://vay.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://cqt.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://tpi.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ckw.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://lmq.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://yiy.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://tva.sysykeji.top

[H07] 断言
来源：http://nsu.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://cox.yangfankeji.com

PHP:  assert($x > 0);
来源：http://gas.yj202588.top

JS:   console.assert(x > 0);
来源：http://dph.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://jdz.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://ndo.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dfi.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tix.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://gva.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://gbu.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://fbx.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jwg.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://tef.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ucd.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qij.zhaomingkeji.xyz

Go:   err.Error()
来源：http://etz.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://cmw.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://mre.daria6918.cn

[H09] 带错误码的异常
来源：http://ycq.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mww.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wwd.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wdj.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jzr.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://osm.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fxn.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://tcz.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fei.shuidangran.top

[H10] 资源自动释放
来源：http://npw.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xdz.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://klz.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zow.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xlr.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zre.yj202588.top

Go:   defer f.Close()
来源：http://tln.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uqx.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ivh.zdbjq.cn

================================================================================
来源：http://ena.xylfe.cn

I. 正则表达式
来源：http://nkn.xuanzx.com

================================================================================
来源：http://umz.ydjk.org.cn

[I01] 判断是否匹配
来源：http://gza.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qpf.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ocf.vehdjk.com

JS:   /\d+/.test(s)
来源：http://uuv.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://axn.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qzo.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tdp.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://iez.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://guw.cheryme.top

[I02] 提取所有匹配
来源：http://lgl.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://jbb.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vqt.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fhz.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://efm.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aaa.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pkz.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://pyn.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ync.bjfxy.top

[I03] 提取捕获分组
来源：http://alc.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ioa.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gmb.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pha.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xwb.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kdj.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kkp.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://epu.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rab.aibaodan.cn

[I04] 正则替换
来源：http://lxx.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tio.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ajy.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://obr.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://tro.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://wez.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://twv.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nom.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ccv.yongpay.top

[I05] 按正则拆分
来源：http://msj.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://cdm.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tzn.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://zgv.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://odc.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://ykw.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tip.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://two.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wyh.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wvc.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pkw.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bwc.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jtz.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ncd.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oyl.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kmx.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vsi.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sri.tanke756.top

[I07] 忽略大小写与多行模式
来源：http://lbi.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://epq.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xnc.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pfy.aizwys.cn

TS:   /error/gim
来源：http://lih.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vme.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xoz.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://efd.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hee.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://ccn.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zas.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qdm.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://top.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yur.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bmo.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://goi.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pfp.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aab.quarkkingdee.top

================================================================================
来源：http://lcj.cdnleiting.top

J. 日期与时间
来源：http://vtu.guowangkeji.top

================================================================================
来源：http://spk.yj20258888.top

[J01] 获取当前时间
来源：http://zuf.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://opd.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dof.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://jdw.xylfe.cn

TS:   new Date();  Date.now()
来源：http://ynr.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://umt.hnqzz.top

Go:   time.Now()
来源：http://pzw.vqdsnc.cn

Ruby: Time.now
来源：http://saa.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jwi.chenzaomai.com

[J02] 格式化输出
来源：http://tbb.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qlj.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jcc.fktsv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uda.ybcxt.top

TS:   d.toISOString()
来源：http://nxd.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://usm.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pbp.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rso.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zmr.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://mgo.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dcm.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://whx.sweek.top

JS:   new Date("2024-01-02")
来源：http://pjs.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://klp.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cwm.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vbw.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://hkw.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://msa.ydzc1.top

[J04] 时间戳与日期互转
来源：http://yjz.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ksh.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yry.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qhr.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bvt.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eks.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wek.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yur.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nkk.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://czf.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://eva.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dol.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pqo.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rke.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://pgv.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nkj.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://vag.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oxo.ppjwa.cn

[J06] 计算两时间之差
来源：http://nvm.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://vpx.sweek.top

PHP:  $end->diff($start)->days;
来源：http://gdz.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fcp.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pvx.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://dtf.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://oks.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://nfm.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://zyi.zhongyouzk.top

[J07] 比较两个日期
来源：http://cnx.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://lol.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qym.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://cae.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fkn.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vny.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rig.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://aek.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://vst.52xcode.cn

[J08] 提取年月日与星期
来源：http://wyh.hnxiangtu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vnf.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wly.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gmu.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://onu.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://utr.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nja.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uqu.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xbk.zhiwuduotai.top

[J09] 时区处理
来源：http://nlo.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gvf.xziqi.cn


<!-- 参考信息 -->