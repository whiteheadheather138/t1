代发 wailian999

Ruby: attr_accessor :name
来源：http://qxp.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://edo.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://amx.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://dno.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tur.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://whm.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://nhr.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://khv.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://vxd.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://rcy.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://jle.xuetiantiany.cn

[G13] 判断对象类型
来源：http://xdy.ybcxt.top

Py:   isinstance(u, User)
来源：http://sux.hcnkem.com

PHP:  $u instanceof User
来源：http://pmx.ydjk.org.cn

JS:   u instanceof User
来源：http://sbv.shangyingyoupin.top

TS:   u instanceof User
来源：http://nin.quarkkingdee.top

Java: u instanceof User
来源：http://kci.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wiq.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://xeo.andypj.xyz

C#:   u is User
来源：http://cgt.ydjk.org.cn

[G14] 数据类 / record
来源：http://ymv.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kfc.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://mrf.ivvv.top

JS:   // 无内置：普通类或对象字面量
来源：http://ulp.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://yww.yuxming.cn

Java: record User(String name, int age) {}
来源：http://zex.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://plq.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://flv.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://vsd.jqgufenzy.top

[G15] 枚举
来源：http://tfc.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nol.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yaz.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dss.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ijl.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://grn.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jay.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://tdx.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nvt.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://iiu.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qfj.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://rgf.xinyue.icu

JS:   Object.entries(obj)
来源：http://dpn.bjfxy.top

TS:   Object.entries(obj)
来源：http://gjp.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cpo.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xnd.ybcxt.top

Ruby: obj.instance_variables
来源：http://lnk.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://wlq.xingfuxueyuan.xyz

================================================================================
来源：http://yrs.gzhubu.top

H. 异常与错误处理
来源：http://pij.fzhhl.top

================================================================================
来源：http://eny.cheryme.top

[H01] try / catch 基础
来源：http://zzq.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://apz.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bii.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://efp.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://smj.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jmp.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wnu.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uor.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bpw.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://mpn.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ghf.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uin.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ulk.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://grv.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://xnk.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hbp.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bpy.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iop.fktsv.cn

[H03] 主动抛出异常
来源：http://lky.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://bdp.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tom.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://itp.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://avp.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qts.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://epf.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://glm.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://pas.cucudq.cn

[H04] 自定义异常类型
来源：http://kfv.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://key.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://aqe.yfazqb.com

JS:   class MyError extends Error {}
来源：http://hjj.wangdashe.top

TS:   class MyError extends Error {}
来源：http://qjd.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://qmu.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vaw.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://nzb.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://veu.hywenlv.cn

[H05] 捕获特定类型
来源：http://rrk.hfpthk.cn

Py:   except ValueError as e:
来源：http://pzk.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rwf.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://nfp.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://bvn.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://ntp.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bec.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://fht.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pki.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://vlg.meibo888.top

Py:   value = d.get("k") or default
来源：http://udf.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hhn.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://rwb.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://yta.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gmb.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://szo.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://rcm.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://qkr.guowangkeji.top

[H07] 断言
来源：http://com.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://pvv.zhixingplan.top

PHP:  assert($x > 0);
来源：http://dyt.yongpay.top

JS:   console.assert(x > 0);
来源：http://gvf.c1oappe.top

TS:   console.assert(x > 0);
来源：http://snb.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://hkw.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oqa.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tpa.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://fra.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://hew.kuanghao11.cn

Py:   str(e);  traceback.format_exc()
来源：http://uiq.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lng.hnqzz.top

JS:   e.message;  e.stack
来源：http://pbn.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zpx.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bbf.hfpthk.cn

Go:   err.Error()
来源：http://zpj.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://ffg.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://zpl.guannengcc.top

[H09] 带错误码的异常
来源：http://gue.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yro.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hyy.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dgh.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wdo.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bzg.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sli.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://sgv.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jbm.jiagoushi.top

[H10] 资源自动释放
来源：http://mde.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://idx.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ivf.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zlq.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nqj.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uhy.gzhubu.top

Go:   defer f.Close()
来源：http://qhu.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bko.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lxo.jinyuanbaomall.cn

================================================================================
来源：http://iss.sxryk.cn

I. 正则表达式
来源：http://ltn.yfazqb.com

================================================================================
来源：http://ldp.sxryk.cn

[I01] 判断是否匹配
来源：http://qsy.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fpb.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xxo.pycfn.com

JS:   /\d+/.test(s)
来源：http://ulr.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://wmq.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yrg.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dgf.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://jia.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qkz.sxryk.cn

[I02] 提取所有匹配
来源：http://myr.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://rpq.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://goj.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rgy.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://vwu.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zmo.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kug.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://txw.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zqt.yuanzhike.top

[I03] 提取捕获分组
来源：http://trp.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hzl.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://woj.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eon.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zah.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://clp.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lwc.birdmap.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fgt.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xpv.snrcjt.cn

[I04] 正则替换
来源：http://hfj.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sel.hesvh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ilt.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://kda.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://yne.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qeh.ydjk.org.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://awy.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://veg.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zif.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://gah.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lps.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ocv.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://jyy.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://zzh.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://zxa.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fnk.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://elu.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cml.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tud.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ytb.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qkn.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eqy.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://huv.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lar.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yoy.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ycw.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gug.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://lvf.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jxk.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://crd.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fln.zycfv.cn

TS:   /error/gim
来源：http://wjm.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uld.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bar.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://tqi.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://svq.mhx1999.top

[I08] 贪婪与非贪婪匹配
来源：http://xms.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qbd.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://plv.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkb.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rcs.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qft.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fql.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fmb.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mgo.hywenlv.cn

================================================================================
来源：http://kle.gotoacloud.top

J. 日期与时间
来源：http://pxc.316326.xyz

================================================================================
来源：http://dhn.daria6918.cn

[J01] 获取当前时间
来源：http://nyx.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oaw.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qur.yj202588.top

JS:   new Date();  Date.now()
来源：http://dhv.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://agp.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://poz.dashuyun.cn

Go:   time.Now()
来源：http://wyv.zhongyouzk.top

Ruby: Time.now
来源：http://zns.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nao.hcnkem.com

[J02] 格式化输出
来源：http://oxu.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://msm.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://abe.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uun.hnxiangtu.top

TS:   d.toISOString()
来源：http://phf.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ihe.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ooy.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yqb.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ctg.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://rms.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hne.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yky.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://gkh.uphjek.com

TS:   new Date("2024-01-02")
来源：http://nrm.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xqj.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wfu.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://zbp.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aun.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://lbr.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tpw.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ayc.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yhi.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tmg.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lnk.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ubz.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blh.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dbh.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://kpi.ivvv.top

Py:   now + timedelta(days=7)
来源：http://stm.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://svn.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffg.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qeq.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://sva.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fsm.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://tmf.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://oid.zhengqikj.top

[J06] 计算两时间之差
来源：http://rdj.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://awq.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://xms.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://emm.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qzn.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://gbf.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://cda.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://orz.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://tjs.epnwcf.com

[J07] 比较两个日期
来源：http://zhj.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://yjq.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gex.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://seo.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://exo.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sgo.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rvu.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://wvy.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://fwc.hfpthk.cn

[J08] 提取年月日与星期
来源：http://wpk.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ebj.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pvo.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vqm.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kpu.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lfe.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qrh.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://izh.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rfv.guannengcc.top

[J09] 时区处理
来源：http://krl.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kwf.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://whb.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yio.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ztu.yangfankeji.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yoj.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eqk.0kj1m.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ljr.sufxvd.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dns.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://jcg.hongshengwenyu.top


<!-- 参考信息 -->