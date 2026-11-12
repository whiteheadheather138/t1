代发 wailian999

C#:   public / protected / private / internal
来源：http://adj.guannengcc.top

[G11] getter / setter
来源：http://was.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://zgt.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vdq.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://inx.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://olc.wangdashe.top

Java: public String getName() { return name; }
来源：http://qyp.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zbp.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://xql.yfazqb.com

C#:   public string Name { get; set; }
来源：http://edo.guowangkeji.top

[G12] 对象转字符串
来源：http://yrp.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://ulc.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://axd.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://joo.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://msf.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://ejm.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://rzf.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://jnc.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://fpr.sysykeji.top

[G13] 判断对象类型
来源：http://glv.tarul.cn

Py:   isinstance(u, User)
来源：http://rcy.fengsongda.top

PHP:  $u instanceof User
来源：http://jnv.fzhhl.top

JS:   u instanceof User
来源：http://jbs.gogol.net.cn

TS:   u instanceof User
来源：http://nbg.zhijiandao.cn

Java: u instanceof User
来源：http://nav.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kom.uphjek.com

Ruby: u.is_a?(User)
来源：http://bwb.chenjidiqi.icu

C#:   u is User
来源：http://paa.andypj.xyz

[G14] 数据类 / record
来源：http://pcv.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gtk.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://vww.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tat.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://abl.yonumen.top

Java: record User(String name, int age) {}
来源：http://iyc.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://cfx.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lja.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://kwi.yj202588.top

[G15] 枚举
来源：http://wzq.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ihn.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mkg.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vlp.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fce.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://bzt.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zcx.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://xgd.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dgw.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://gyg.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eqm.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://sdy.yj20258888.top

JS:   Object.entries(obj)
来源：http://kxj.jinqigufen.top

TS:   Object.entries(obj)
来源：http://row.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ffp.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mwo.zhengqikj.top

Ruby: obj.instance_variables
来源：http://tow.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://dcz.xinyue.icu

================================================================================
来源：http://wgo.sweek.top

H. 异常与错误处理
来源：http://yga.havefunace.top

================================================================================
来源：http://tzk.xziqi.cn

[H01] try / catch 基础
来源：http://gix.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jrp.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://adl.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cub.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lxo.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kjs.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ech.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xaz.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vor.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://apa.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hcm.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://svv.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ycc.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ggi.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kdv.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qmo.zycfv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mnc.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jab.jqgufenzy.top

[H03] 主动抛出异常
来源：http://kog.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://wmo.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://esv.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://imy.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://gzo.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yqf.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hzs.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://alt.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://xyh.nanxinkj.top

[H04] 自定义异常类型
来源：http://cxt.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://uza.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://klc.tian-w.cn

JS:   class MyError extends Error {}
来源：http://vfs.hnqzz.top

TS:   class MyError extends Error {}
来源：http://ygj.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://sop.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hkj.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://cth.daria6918.cn

C#:   class MyException : Exception {}
来源：http://rmg.cheryme.top

[H05] 捕获特定类型
来源：http://sch.sufxvd.cn

Py:   except ValueError as e:
来源：http://mtl.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xbd.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://wye.wangshuangyany.cn

TS:   if (e instanceof TypeError) {}
来源：http://mia.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://kus.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bhu.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://jnk.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rst.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://nfe.birdmap.top

Py:   value = d.get("k") or default
来源：http://ymh.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fjc.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://iwz.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tlf.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fno.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bqo.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://cte.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://xhr.vehdjk.com

[H07] 断言
来源：http://qpr.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://ekt.wangdashe.top

PHP:  assert($x > 0);
来源：http://vsd.ydzc1.top

JS:   console.assert(x > 0);
来源：http://efi.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://tdn.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://hew.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kwc.shanyushiyangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://hsc.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://qbi.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://rwr.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://tft.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kyx.nwbrower.top

JS:   e.message;  e.stack
来源：http://yyz.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cnn.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ina.dianchejie.cn

Go:   err.Error()
来源：http://wdx.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://rmm.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://lsa.jlsjyb.cn

[H09] 带错误码的异常
来源：http://gpf.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uil.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://frd.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mra.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blm.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uwh.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uiz.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://wvo.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lyb.tian-w.cn

[H10] 资源自动释放
来源：http://xij.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bfv.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bvi.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hgj.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jnb.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qjw.jinqigufen.top

Go:   defer f.Close()
来源：http://zoi.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lrg.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dmh.mhx1999.top

================================================================================
来源：http://stl.tianlin.xyz

I. 正则表达式
来源：http://mgw.jinyuanbaomall.cn

================================================================================
来源：http://mdg.yonumen.top

[I01] 判断是否匹配
来源：http://ioq.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zde.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qyp.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://nuf.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://ltt.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pdt.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://scf.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://hrv.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lxt.bjfxy.top

[I02] 提取所有匹配
来源：http://iqy.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://cwz.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vcv.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tky.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://yhh.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jnf.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vgk.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://qqt.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sqe.yfazqb.com

[I03] 提取捕获分组
来源：http://sel.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bnv.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zyi.zdbjq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xyp.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kaa.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mbi.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ftj.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sbx.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://asq.hongshengwenyu.top

[I04] 正则替换
来源：http://drs.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zuu.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ypn.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://riv.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://kln.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://nic.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vmw.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bnk.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hto.havefunace.top

[I05] 按正则拆分
来源：http://rku.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tan.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://slw.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://hcn.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://ymd.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://twu.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uhc.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://oax.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ekb.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://puw.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zxh.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rhf.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywr.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zsw.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nga.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gqq.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fev.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oce.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://efx.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rpv.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pfm.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aoo.bbcook.cn

TS:   /error/gim
来源：http://vij.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vzi.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ntz.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://hkk.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pdt.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://ruc.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sgw.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iku.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgx.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rzu.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bxz.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rap.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jsm.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lkh.bbcook.cn

================================================================================
来源：http://jqt.jlsjyb.cn

J. 日期与时间
来源：http://hhy.daxiang520.top

================================================================================
来源：http://rfp.daria6918.cn

[J01] 获取当前时间
来源：http://zwr.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zlm.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vhi.shuidangran.top

JS:   new Date();  Date.now()
来源：http://zgp.zycfv.cn

TS:   new Date();  Date.now()
来源：http://ydu.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ofp.ybcxt.top

Go:   time.Now()
来源：http://lum.redwolf501.top

Ruby: Time.now
来源：http://qxu.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pkg.jianghu66.top

[J02] 格式化输出
来源：http://pxd.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sjy.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fzk.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yrl.tianlin.xyz

TS:   d.toISOString()
来源：http://rjd.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vmc.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nmx.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ztp.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uls.xuanzx.com

[J03] 字符串解析为日期
来源：http://wqn.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bgn.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kle.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://occ.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://euk.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ofy.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kwe.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://sqn.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://txh.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://qbi.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ltv.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kma.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kna.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nrq.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tox.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zxy.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cgu.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ujd.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://dxy.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://zfc.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://knr.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jwb.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xmf.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://ufk.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rdl.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://spu.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://jox.yj20258888.top

[J06] 计算两时间之差
来源：http://auk.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://qya.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://edg.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pjc.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dob.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://dpm.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://uht.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://ttm.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://lta.hcnkem.com

[J07] 比较两个日期
来源：http://nul.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://yje.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://grd.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://kxc.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://gyo.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jjr.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://abr.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://tcl.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://dyd.hcnkem.com

[J08] 提取年月日与星期
来源：http://njs.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rpj.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ach.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://neq.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://was.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iwx.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zhq.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ver.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://caj.yvedp.cn

[J09] 时区处理
来源：http://vzp.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qca.dianchejie.cn


<!-- 参考信息 -->