代发 wailian999

C#:   public / protected / private / internal
来源：http://yds.gogol.net.cn

[G11] getter / setter
来源：http://svh.jianghu66.top

Py:   @property 与 @x.setter
来源：http://xyx.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zir.ydzc1.top

JS:   get name() { return this._name; }
来源：http://xqz.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://mix.yongpay.top

Java: public String getName() { return name; }
来源：http://nnd.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://tfh.fengsongda.top

Ruby: attr_accessor :name
来源：http://axv.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://toi.sweek.top

[G12] 对象转字符串
来源：http://huk.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://tah.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yyt.ydzc1.top

JS:   toString() { return this.name; }
来源：http://jzl.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://dzh.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://cai.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://sqn.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://cpa.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://ahd.daxiang520.top

[G13] 判断对象类型
来源：http://aij.zdqjudy.top

Py:   isinstance(u, User)
来源：http://tyq.hcnkem.com

PHP:  $u instanceof User
来源：http://wbm.chenjidiqi.icu

JS:   u instanceof User
来源：http://nes.xylfe.cn

TS:   u instanceof User
来源：http://pbz.hesvh.cn

Java: u instanceof User
来源：http://rxn.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jrc.xziqi.cn

Ruby: u.is_a?(User)
来源：http://wti.jinqigfzy.top

C#:   u is User
来源：http://uzd.gaohongyu789.top

[G14] 数据类 / record
来源：http://iyu.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fyd.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://ddl.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://agl.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://xml.zhoulong.xyz

Java: record User(String name, int age) {}
来源：http://dfh.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://vud.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ear.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://frl.sxryk.cn

[G15] 枚举
来源：http://sog.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zqc.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wwu.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rzz.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fui.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://pps.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mcr.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://spe.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gwz.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://wkn.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fds.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://ked.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://ery.dianchejie.cn

TS:   Object.entries(obj)
来源：http://jhh.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bkl.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://wwc.yj20258.top

Ruby: obj.instance_variables
来源：http://nha.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://iui.shanyushiyangkeji.top

================================================================================
来源：http://pej.yangfankeji.com

H. 异常与错误处理
来源：http://xgu.0kj1m.cn

================================================================================
来源：http://pxd.havefunace.top

[H01] try / catch 基础
来源：http://soe.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gua.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hah.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://apv.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jzx.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lut.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mdn.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://znb.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lwt.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://nyk.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://ike.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eha.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gsf.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://adm.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://qrv.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://raz.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zpp.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yhd.cucudq.cn

[H03] 主动抛出异常
来源：http://qec.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://gvi.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mvt.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://olz.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://tbt.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oqt.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxo.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xhf.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://tbz.cheryme.top

[H04] 自定义异常类型
来源：http://zud.yj20258.top

Py:   class MyError(Exception): pass
来源：http://qpe.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://wzl.guannengcc.top

JS:   class MyError extends Error {}
来源：http://vep.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://avi.ppjwa.cn

Java: class MyException extends RuntimeException {}
来源：http://kwz.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jkm.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://daq.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://ccb.9152youxi.cn

[H05] 捕获特定类型
来源：http://zgq.yfazqb.com

Py:   except ValueError as e:
来源：http://hep.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ldk.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://tgo.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://ris.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://uup.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wdh.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://hnz.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bgp.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://fyw.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://qnp.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dhb.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://ouq.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pvz.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ytz.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gtn.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://kxz.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://gtk.svipenyu.cn

[H07] 断言
来源：http://wut.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://ptq.yfazqb.com

PHP:  assert($x > 0);
来源：http://rci.yj20258888.top

JS:   console.assert(x > 0);
来源：http://jew.yfazqb.com

TS:   console.assert(x > 0);
来源：http://ibv.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://nyd.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dxe.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://czx.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://dmh.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://azg.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://ntm.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://axq.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://fpb.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kvs.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://iwt.zhiwuduotai.top

Go:   err.Error()
来源：http://gja.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://iku.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://lxd.tianlin.xyz

[H09] 带错误码的异常
来源：http://kic.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://unw.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nha.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kmj.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uuk.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://evz.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ngw.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kwn.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fqb.cdnleiting.top

[H10] 资源自动释放
来源：http://qvg.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vdw.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fgm.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xrk.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pag.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ldt.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://ugo.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ivk.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xut.xuanzx.com

================================================================================
来源：http://vjg.haohaochexian.top

I. 正则表达式
来源：http://ngs.cashguo.top

================================================================================
来源：http://uac.ppjwa.cn

[I01] 判断是否匹配
来源：http://fsl.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nnv.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://zvh.sweek.top

JS:   /\d+/.test(s)
来源：http://kgi.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://hgu.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://alj.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://scu.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://exu.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nnp.yj20258888.top

[I02] 提取所有匹配
来源：http://qmi.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://hbd.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://acu.aibaodan.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dof.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://lim.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://swm.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nah.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://wht.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fkg.sufxvd.cn

[I03] 提取捕获分组
来源：http://nao.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://few.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tfg.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kuh.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://apw.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://keq.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rpy.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ymn.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://don.aibaodan.cn

[I04] 正则替换
来源：http://wrm.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aap.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sia.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://nph.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://hau.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://izv.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qah.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://alx.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qok.ppjwa.cn

[I05] 按正则拆分
来源：http://qqo.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://thr.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jkx.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://blj.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://rqi.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://tbc.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rhz.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://ujk.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pbc.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pwh.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uld.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ody.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qjj.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ovh.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oer.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ffo.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jce.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zeh.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://wke.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://imq.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uma.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iks.ydjk.org.cn

TS:   /error/gim
来源：http://opd.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://igc.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://erx.meibo888.top

Ruby: s.scan(/error/i)
来源：http://tqc.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jsw.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://xnc.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bna.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ggr.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sbj.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dxa.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fet.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aay.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jly.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ukt.yangfankeji.com

================================================================================
来源：http://pmm.daxiang520.top

J. 日期与时间
来源：http://vso.wangdashe.top

================================================================================
来源：http://www.havefunace.top

[J01] 获取当前时间
来源：http://uar.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xav.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sfz.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://ecv.pycfn.com

TS:   new Date();  Date.now()
来源：http://ajc.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ryh.pengpengdd.cyou

Go:   time.Now()
来源：http://hsv.tanke756.top

Ruby: Time.now
来源：http://drw.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ixl.ppjwa.cn

[J02] 格式化输出
来源：http://qdx.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uzp.mhx1999.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://skf.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://odt.xziqi.cn

TS:   d.toISOString()
来源：http://jpf.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hrm.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gud.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://shc.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jjg.hfpthk.cn

[J03] 字符串解析为日期
来源：http://rqe.yj20258888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ylv.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uvl.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://ejv.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://bao.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://ugc.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wfk.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://mvm.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kdx.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://ptw.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://luu.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jaa.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nks.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://agq.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ltg.jlsjyb.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jrw.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zrw.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ruj.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://ntg.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://bgy.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ump.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmq.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rty.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://svn.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cgt.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://vgb.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://zsb.0kj1m.cn

[J06] 计算两时间之差
来源：http://zmh.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://gwi.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://ojo.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wpe.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tbx.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://szm.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://xyt.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://ikt.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://flw.hfpthk.cn

[J07] 比较两个日期
来源：http://thz.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://iuf.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qxr.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://ulk.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://wdn.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zru.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://itm.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://zln.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://hou.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://nsv.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pbn.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zrk.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pjv.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rlk.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nqn.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qij.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mhj.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dcz.yfazqb.com

[J09] 时区处理
来源：http://sws.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tvj.ydjk.org.cn


<!-- 参考信息 -->