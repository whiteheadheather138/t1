代发 wailian999

JS:   get name() { return this._name; }
来源：http://kci.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://pte.zdbjq.cn

Java: public String getName() { return name; }
来源：http://zzu.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rek.c1oappe.top

Ruby: attr_accessor :name
来源：http://vdh.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://hcm.chenzaomai.com

[G12] 对象转字符串
来源：http://wdh.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://plq.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gql.hnqzz.top

JS:   toString() { return this.name; }
来源：http://xfo.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://jeg.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://rkh.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://cvv.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://omq.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://cly.gaohongyu789.top

[G13] 判断对象类型
来源：http://zkw.tian-w.cn

Py:   isinstance(u, User)
来源：http://elh.yvedp.cn

PHP:  $u instanceof User
来源：http://ybq.chenlongwang.top

JS:   u instanceof User
来源：http://ufe.meibo888.top

TS:   u instanceof User
来源：http://svp.tian-w.cn

Java: u instanceof User
来源：http://frw.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://flp.yongpay.top

Ruby: u.is_a?(User)
来源：http://goz.jinghuilouyu.cn

C#:   u is User
来源：http://tbb.yvedp.cn

[G14] 数据类 / record
来源：http://cep.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ymz.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://mga.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://zgt.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://zbi.yfazqb.com

Java: record User(String name, int age) {}
来源：http://tet.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://ojk.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mll.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://vee.xingfuxueyuan.xyz

[G15] 枚举
来源：http://bzf.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zga.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://kov.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uqz.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kto.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://fbo.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xnx.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://vgp.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dpf.birdmap.top

[G16] 对象转数组 / 字典
来源：http://gws.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zwu.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://wpw.chenzaomai.com

JS:   Object.entries(obj)
来源：http://gyf.dianchejie.cn

TS:   Object.entries(obj)
来源：http://bwk.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kvk.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://lmg.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://yfc.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://nyr.gotoacloud.top

================================================================================
来源：http://ouw.fengsongda.top

H. 异常与错误处理
来源：http://fzo.ppjwa.cn

================================================================================
来源：http://sgn.wangshuangyany.cn

[H01] try / catch 基础
来源：http://htd.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jdt.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mwj.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vjr.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fbj.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ago.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kiq.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wqq.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nbg.andypj.xyz

[H02] finally / ensure 收尾
来源：http://emq.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://dhb.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ucn.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qeh.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kxc.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://lxx.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rcq.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://cnh.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tva.yj202588.top

[H03] 主动抛出异常
来源：http://flm.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://tyn.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ryd.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://pgz.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://nek.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://yts.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://imm.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wam.zhaomingkeji.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://kdo.yfazqb.com

[H04] 自定义异常类型
来源：http://zvo.tarul.cn

Py:   class MyError(Exception): pass
来源：http://uoq.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fxo.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://tyu.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://wzl.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://vzo.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tnz.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://kaq.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://off.tanke756.top

[H05] 捕获特定类型
来源：http://vme.gogol.net.cn

Py:   except ValueError as e:
来源：http://hdr.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jyt.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://emr.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://djh.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://dql.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cti.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://yqh.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wjn.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://flv.jianghu66.top

Py:   value = d.get("k") or default
来源：http://hxs.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://fnw.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://kyr.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://azv.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ncm.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://urt.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://tes.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://luy.zdqjudy.top

[H07] 断言
来源：http://hti.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://gga.yj202588.top

PHP:  assert($x > 0);
来源：http://yow.hcnkem.com

JS:   console.assert(x > 0);
来源：http://qux.pycfn.com

TS:   console.assert(x > 0);
来源：http://bfs.dianchejie.cn

Java: assert x > 0 : "必须为正";
来源：http://osv.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://svz.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://igi.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://yla.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://bro.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://upl.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mga.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://zuy.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://onc.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://hrg.hywenlv.cn

Go:   err.Error()
来源：http://lap.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://qpu.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://zwr.jyoumei.cn

[H09] 带错误码的异常
来源：http://gxd.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ewf.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://has.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://icx.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fmp.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ius.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://syq.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://ikm.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rma.pycfn.com

[H10] 资源自动释放
来源：http://meu.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://cxo.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zvh.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uos.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pqe.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eds.yuxming.cn

Go:   defer f.Close()
来源：http://viz.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oho.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ian.birdmap.top

================================================================================
来源：http://ilv.wangshuangyany.cn

I. 正则表达式
来源：http://imq.meibo888.top

================================================================================
来源：http://swg.hammf.cn

[I01] 判断是否匹配
来源：http://hpr.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://etx.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vfl.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://wan.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://wpn.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ekv.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tzo.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://jrk.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wvh.sysykeji.top

[I02] 提取所有匹配
来源：http://alh.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://mdj.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tvj.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://elg.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://ems.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lty.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qra.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://qif.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uiy.zhengqikj.top

[I03] 提取捕获分组
来源：http://mts.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fmr.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oiv.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybi.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://srf.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gnz.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ajn.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mwg.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://spq.shzxlz.cn

[I04] 正则替换
来源：http://zxn.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ysg.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://phu.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://yim.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://xmu.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zlh.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ofs.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fct.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zsw.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://znc.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jnc.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://unc.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://csb.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://jiu.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://zxi.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bza.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jqf.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yyc.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gzd.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://etu.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://azh.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aui.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jar.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cec.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ehb.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fpu.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rvb.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://qrq.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ivl.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aue.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pjc.tian-w.cn

TS:   /error/gim
来源：http://jwl.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jxx.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://swu.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://onz.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://klr.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://rnr.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://voi.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qke.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://krk.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lvn.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cuq.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ixc.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://djp.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iss.yueranfly.top

================================================================================
来源：http://lkj.tanke756.top

J. 日期与时间
来源：http://zxi.jlsjyb.cn

================================================================================
来源：http://lda.bbcook.cn

[J01] 获取当前时间
来源：http://gfl.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jnj.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iio.bjfxy.top

JS:   new Date();  Date.now()
来源：http://pjn.mhx1999.top

TS:   new Date();  Date.now()
来源：http://oyl.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://fyv.zycfv.cn

Go:   time.Now()
来源：http://pkn.xuetiantiany.cn

Ruby: Time.now
来源：http://nqg.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://djc.zhiwuduotai.top

[J02] 格式化输出
来源：http://wue.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vou.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fpd.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tzb.wangshuangyany.cn

TS:   d.toISOString()
来源：http://dqv.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fjh.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mwq.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ffq.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yzf.yj20258888.top

[J03] 字符串解析为日期
来源：http://ajs.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iyi.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pdb.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://tvo.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://onf.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://pzm.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://glq.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://nya.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nfm.wangdashe.top

[J04] 时间戳与日期互转
来源：http://qic.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xmt.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qkg.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pvy.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lew.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ckj.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fgy.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://foe.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qqg.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://jpy.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://pap.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bfw.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gyx.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pnd.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://kdc.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ybd.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://mvp.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://xwv.bjfxy.top

[J06] 计算两时间之差
来源：http://hdw.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://oho.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://akg.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xhz.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jpe.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://snd.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://cti.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://nya.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://gfl.shuidangran.top

[J07] 比较两个日期
来源：http://cil.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://jwq.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://csf.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://ijc.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://zrc.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dtd.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aet.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://amb.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://zmp.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://ddn.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kku.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://unl.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lcg.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://okc.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://usj.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rzg.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://alj.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://exw.dashuyun.cn

[J09] 时区处理
来源：http://tqc.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fvn.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dxa.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kur.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bev.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ufx.chenlongwang.top


<!-- 参考信息 -->