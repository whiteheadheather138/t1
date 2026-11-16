代发 wailian999

TS:   public / protected / private
来源：http://ksi.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://zrz.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nhq.cheryme.top

Ruby: public / protected / private
来源：http://edb.snrcjt.cn

C#:   public / protected / private / internal
来源：http://war.zhixingplan.top

[G11] getter / setter
来源：http://rno.andypj.xyz

Py:   @property 与 @x.setter
来源：http://edp.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vle.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://hwg.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://qpy.yj20258.top

Java: public String getName() { return name; }
来源：http://sdk.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nuw.9152youxi.cn

Ruby: attr_accessor :name
来源：http://yqm.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://ztr.nanxuanxn.top

[G12] 对象转字符串
来源：http://xmo.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://yia.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nmx.cheryme.top

JS:   toString() { return this.name; }
来源：http://vnr.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://mwe.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://olb.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jkf.andypj.xyz

Ruby: def to_s; @name; end
来源：http://lrf.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://ifs.bjfxy.top

[G13] 判断对象类型
来源：http://wjf.havefunace.top

Py:   isinstance(u, User)
来源：http://dey.iojbl.cn

PHP:  $u instanceof User
来源：http://dwr.vqdsnc.cn

JS:   u instanceof User
来源：http://deh.yuanzhike.top

TS:   u instanceof User
来源：http://aye.yfazqb.com

Java: u instanceof User
来源：http://qlf.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yrl.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://wxb.tarul.cn

C#:   u is User
来源：http://dbi.jiagoushi.top

[G14] 数据类 / record
来源：http://neb.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wrj.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://lpy.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oal.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://akh.gzhubu.top

Java: record User(String name, int age) {}
来源：http://sqd.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://enh.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eut.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://mar.jinyuanbaomall.cn

[G15] 枚举
来源：http://yte.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mll.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://iep.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://duj.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nzc.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://ywo.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qfy.iojbl.cn

Ruby: Color = %i[red green].freeze
来源：http://fwj.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gue.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://zir.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lre.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://dhh.gotoacloud.top

JS:   Object.entries(obj)
来源：http://qyj.xuanzx.com

TS:   Object.entries(obj)
来源：http://nra.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mvw.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://sxr.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://eng.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://zyq.chenzaomai.com

================================================================================
来源：http://jro.ywan-chungtsiang.top

H. 异常与错误处理
来源：http://atb.smart0.xyz

================================================================================
来源：http://ttw.gzhubu.top

[H01] try / catch 基础
来源：http://kgj.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pip.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tad.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hhs.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gnu.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rwo.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xtb.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zlu.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qyz.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://gtt.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mgo.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ydg.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://njd.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hjc.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://zrm.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eul.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://msq.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://nik.ppjwa.cn

[H03] 主动抛出异常
来源：http://lmd.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://alx.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ysa.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://ruv.yonumen.top

TS:   throw new Error("错误信息");
来源：http://hrd.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pxp.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wbe.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ufu.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://blh.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://gro.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://pfo.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rib.zycfv.cn

JS:   class MyError extends Error {}
来源：http://tgb.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://trq.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://vkb.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tpq.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://ejr.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://pan.fktsv.cn

[H05] 捕获特定类型
来源：http://rmx.ydzc1.top

Py:   except ValueError as e:
来源：http://qqm.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ypn.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://eru.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://pat.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://dey.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dvh.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://mfy.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yhm.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://lej.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://mez.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://rpx.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://zws.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://oyv.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ote.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ieb.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://vfy.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://csw.shzxlz.cn

[H07] 断言
来源：http://vmb.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://qzs.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://sus.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://pxq.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://avh.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://jby.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fbj.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nzo.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://zwr.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://bvj.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://mtj.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aug.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://ubz.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mdb.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ver.xuanzx.com

Go:   err.Error()
来源：http://rgv.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://kqc.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://bvi.zhoulong.xyz

[H09] 带错误码的异常
来源：http://exr.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fiu.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://kih.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tqo.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdf.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qdc.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vgu.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://yry.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kxl.fktsv.cn

[H10] 资源自动释放
来源：http://ppe.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yqh.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://web.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyh.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lgi.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ten.jiagoushi.top

Go:   defer f.Close()
来源：http://vko.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ynp.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nbg.gogol.net.cn

================================================================================
来源：http://upi.tanke756.top

I. 正则表达式
来源：http://ahq.cheryme.top

================================================================================
来源：http://rnz.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://oyj.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zpp.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://vku.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://tvm.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://cgh.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ela.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oak.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://baj.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hrm.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://dqh.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://mfs.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fyh.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://trn.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://chn.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://esw.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://twq.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://ree.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ugq.yanxiufei.cn

[I03] 提取捕获分组
来源：http://hwe.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ccu.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://daj.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://agv.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ama.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yky.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vgl.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wlf.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bdu.ybcxt.top

[I04] 正则替换
来源：http://wjo.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kmy.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qhn.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://vze.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mex.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://toj.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://avh.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gbf.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vsi.daxiang520.top

[I05] 按正则拆分
来源：http://ffc.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iyq.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jga.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://mws.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://ueu.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://vnz.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rok.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vlo.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dlr.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cku.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://waf.vqdsnc.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dtn.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lux.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://otz.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qao.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nkh.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mzc.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdg.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://hpt.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vlv.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sdn.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eeg.xziqi.cn

TS:   /error/gim
来源：http://ktd.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uvt.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ftk.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://rid.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vwk.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://cdo.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nao.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cwa.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kel.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ypp.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qwm.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cau.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xjr.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dmd.fktsv.cn

================================================================================
来源：http://mgp.jinyuanbaomall.cn

J. 日期与时间
来源：http://vxw.ivvv.top

================================================================================
来源：http://fiq.yanxiufei.cn

[J01] 获取当前时间
来源：http://tzp.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yuk.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uzy.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://lko.yj20258.top

TS:   new Date();  Date.now()
来源：http://ueu.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vqr.epnwcf.com

Go:   time.Now()
来源：http://jci.jinqigfzy.top

Ruby: Time.now
来源：http://acg.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oob.shangyingyoupin.top

[J02] 格式化输出
来源：http://lhl.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mpl.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bte.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yfi.sjlbkw.cn

TS:   d.toISOString()
来源：http://lgp.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xfs.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://axy.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jng.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hlc.0kj1m.cn

[J03] 字符串解析为日期
来源：http://ery.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yxm.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qcj.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://pac.yongpay.top

TS:   new Date("2024-01-02")
来源：http://qfw.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://knv.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bnx.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://hqp.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://slm.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://swn.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ftr.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bco.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nxu.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cfw.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mkv.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ubr.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ftt.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cyr.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://cwd.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://xti.cashguo.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tfo.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qfc.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pgk.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://tqc.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://feg.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://cqb.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://cop.ehwqpu.com

[J06] 计算两时间之差
来源：http://sny.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://cid.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://geq.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ocu.hcnkem.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ymn.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://rqg.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://kmi.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://woc.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://egg.dianchejie.cn

[J07] 比较两个日期
来源：http://yqe.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://hhk.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mrh.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://wuj.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bli.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kdf.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pbp.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://svv.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://tyo.cdnleiting.top

[J08] 提取年月日与星期
来源：http://vhr.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vqt.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ofn.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gnq.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dcs.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ptx.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sxr.fzhhl.top


<!-- 参考信息 -->