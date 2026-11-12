代发 wailian999

[Q80] 字符串截取
来源：http://jhw.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gke.fehbvm.com

[Q81] 字符串替换
来源：http://qvw.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://onq.cheryme.top

[Q82] 字符长度与字节长度
来源：http://ozh.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gal.xinyue.icu

[Q83] 大小写转换
来源：http://qol.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://anp.cqqwz.cn

[Q84] 去除首尾空格
来源：http://lzq.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://iaw.sysykeji.top

[Q85] 数值取整
来源：http://dvu.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wgy.shzxlz.cn

[Q86] 读取 JSON 字段
来源：http://hcx.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://efr.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://rpx.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mif.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://bjn.hesvh.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rbw.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://epx.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://xwc.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dup.guowangkeji.top

[Q90] 生成序号列
来源：http://ehj.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tvr.uphjek.com

================================================================================
来源：http://vyr.vqdsnc.cn

R. Bash 专题
来源：http://wfm.hnxiangtu.top

================================================================================
来源：http://dqi.yj20258.top

[R01] shebang 与严格模式
来源：http://ssv.jqgufenzy.top

#!/usr/bin/env bash
来源：http://ukz.zhijiandao.cn

set -euo pipefail
来源：http://mnc.c1oappe.top

[R02] 变量赋值与使用
来源：http://qnn.ybcxt.top

name="Tom"; echo "$name"
来源：http://lri.xuanzx.com

[R03] 只读变量
来源：http://hib.chenzaomai.com

readonly PI=3.14
来源：http://xst.zhoulong.xyz

[R04] 位置参数
来源：http://rlq.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://itv.hysaishi.cn

[R05] 参数默认值
来源：http://qdx.redwolf501.top

name="${1:-default}"
来源：http://jrc.yj202588.top

[R06] 判断命令是否存在
来源：http://tlc.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rbv.jinqigufen.top

[R07] if 判断文件
来源：http://kyy.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pho.yvedp.cn

[R08] 数值比较
来源：http://xlc.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pki.hcnkem.com

[R09] 字符串比较
来源：http://auv.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vug.shanyushiyangkeji.top

[R10] 正则匹配
来源：http://fqm.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oss.tarul.cn

[R11] case 多分支
来源：http://ypm.wangshuangyany.cn

case "$1" in
来源：http://ptg.shzxlz.cn

start) echo "启动" ;;
来源：http://wpm.havefunace.top

stop)  echo "停止" ;;
来源：http://hht.birdmap.top

*)     echo "未知命令" ;;
来源：http://hdy.guowangkeji.top

esac
来源：http://eal.wangshuangyany.cn

[R12] for 遍历文件
来源：http://tzo.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://ixr.chenlongwang.top

[R13] for 计数循环
来源：http://kqd.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://ule.tanke756.top

[R14] C 风格 for
来源：http://opf.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oer.yuanzhike.top

[R15] while 逐行读文件
来源：http://wpp.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nus.52xcode.cn

[R16] until 等待条件
来源：http://woy.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://toa.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://kkc.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://wzv.yuxming.cn

[R18] 遍历数组
来源：http://ifs.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oiy.jianghu66.top

[R19] 数组长度
来源：http://vtv.jqgfzy.top

echo "${#arr[@]}"
来源：http://iun.jinqigufen.top

[R20] 关联数组（字典）
来源：http://fow.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hnu.c1oappe.top

[R21] 字符串长度
来源：http://utq.zdbjq.cn

echo "${#s}"
来源：http://kzd.iojbl.cn

[R22] 截取子串
来源：http://ken.hywenlv.cn

echo "${s:0:5}"
来源：http://zbk.ppjwa.cn

[R23] 字符串替换
来源：http://ruj.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mnl.cheryme.top

[R24] 大小写转换
来源：http://sue.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://wgs.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://ykg.yvedp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ewy.yueranfly.top

[R26] 命令替换
来源：http://wgx.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://rar.xuanzx.com

[R27] 算术展开
来源：http://vsm.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://ifx.wangdashe.top

[R28] 浮点运算
来源：http://mev.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://dnj.hammf.cn

[R29] 定义函数
来源：http://dpn.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lzn.vqdsnc.cn

[R30] 函数返回状态码
来源：http://vpa.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://auk.ybcxt.top

[R31] 局部变量
来源：http://jks.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://jlp.jinqigfzy.top

[R32] 参数个数校验
来源：http://sne.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mhy.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://jyp.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bts.ybcxt.top

[R34] 退出时清理
来源：http://ciz.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vma.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://zxq.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ujx.bjfxy.top

[R36] 并发执行多个任务
来源：http://dwb.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jwt.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://kgw.jqgufenzy.top

files=$(ls -1)
来源：http://gwy.sjlbkw.cn

[R38] 管道串联
来源：http://ahb.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://zge.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://mum.yvedp.cn

cmd > out.log 2>&1
来源：http://eic.pycfn.com

[R40] 追加写日志
来源：http://eta.andypj.xyz

echo "log" >> out.log
来源：http://yha.yanxiufei.cn

[R41] 丢弃输出
来源：http://oub.daria6918.cn

cmd >/dev/null 2>&1
来源：http://rqh.yanxiufei.cn

[R42] 输入重定向
来源：http://ojv.chenzaomai.com

wc -l < a.txt
来源：http://hqc.yj20258888.top

[R43] 按名字查找文件
来源：http://lxv.yj202588.top

find . -name "*.log" -type f
来源：http://vbk.guowangkeji.top

[R44] 按修改时间查找
来源：http://wxh.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://eln.fengsongda.top

[R45] 批量删除
来源：http://vml.hnqzz.top

find . -name "*.tmp" -delete
来源：http://sit.yuanzhike.top

[R46] 递归替换文件内容
来源：http://ojs.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cbt.daria6918.cn

[R47] sed 单行替换
来源：http://blm.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bjw.daxiang520.top

[R48] awk 取指定列
来源：http://hqk.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://ljd.cdnleiting.top

[R49] awk 带条件
来源：http://mhs.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rut.yj20258.top

[R50] awk 求和
来源：http://zgh.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://srd.cdnleiting.top

[R51] 排序去重取前几
来源：http://vwh.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fls.c1oappe.top

[R52] 统计行数
来源：http://vrz.ydjk.org.cn

wc -l a.txt
来源：http://mzn.hammf.cn

[R53] 查看文件头与实时尾
来源：http://fdz.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mkc.yueranfly.top

[R54] 比较两个文件
来源：http://omy.9152youxi.cn

diff a.txt b.txt
来源：http://hfy.hfpthk.cn

[R55] 压缩与解压
来源：http://ydn.jinyuanbaomall.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tpg.zdqjudy.top

[R56] 远程拷贝
来源：http://aku.ppjwa.cn

scp file user@host:/path/
来源：http://ose.jinghuilouyu.cn

[R57] 远程执行命令
来源：http://aeq.zhongyouzk.top

ssh user@host 'uptime'
来源：http://thp.fengsongda.top

[R58] 下载文件
来源：http://tpo.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gdd.ctjpmb.com

[R59] 发 POST JSON
来源：http://ahz.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ljc.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://wsz.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vdr.epnwcf.com

[R61] 磁盘占用
来源：http://yap.hammf.cn

df -h;  du -sh *
来源：http://qlu.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://oae.tarul.cn

du -ah . | sort -rh | head -10
来源：http://ssj.chenjidiqi.icu

[R63] 内存与进程
来源：http://vva.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://kck.shzxlz.cn

[R64] 结束进程
来源：http://mqo.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://nwy.ivvv.top

[R65] 查看端口占用
来源：http://pwq.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rtl.snrcjt.cn

[R66] 定时任务
来源：http://aai.yanxiufei.cn

crontab -e;  crontab -l
来源：http://aaa.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://voj.tian-w.cn

openssl rand -hex 16
来源：http://ere.nwbrower.top

[R68] 计算文件校验值
来源：http://fqx.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://fkn.pengpengdd.cyou

[R69] 生成随机密码
来源：http://uvn.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://nro.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://cwn.ydzc1.top

date +%s;  date -d @1700000000
来源：http://xfm.andypj.xyz

[R71] 日期格式化
来源：http://qug.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yuw.ctjpmb.com

[R72] 等待端口就绪
来源：http://vap.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://udu.uphjek.com

[R73] 分割大日志
来源：http://zqr.yonumen.top

split -l 1000 big.log part_
来源：http://chf.shuidangran.top

[R74] 批量重命名
来源：http://jlp.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jzn.xylfe.cn

[R75] 导出环境变量
来源：http://kug.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://mho.yangfankeji.com

[R76] 使用临时文件
来源：http://xwf.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vvs.cucudq.cn

[R77] 读取用户输入
来源：http://nxb.gaohongyu789.top

read -rp "请输入: " ans
来源：http://oob.fengsongda.top

[R78] 交互式菜单
来源：http://myb.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://smw.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://nmp.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uak.xingfuxueyuan.xyz

[R80] 查看脚本执行耗时
来源：http://ovy.nwbrower.top

time ./run.sh
来源：http://ulp.hongshengwenyu.top

================================================================================
来源：http://rwz.ctjpmb.com

S. C / C++ 专题
来源：http://kel.yonumen.top

================================================================================
来源：http://gcn.ctjpmb.com

[S01] C：Hello World
来源：http://dah.snrcjt.cn

#include <stdio.h>
来源：http://bzf.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qps.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://xyh.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://odl.wangshuangyany.cn

[S03] C：读入整数
来源：http://rqz.yonumen.top

int x; scanf("%d", &x);
来源：http://oeb.ppjwa.cn

[S04] C：字符串复制
来源：http://rrj.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://hue.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://fgi.zhongyouzk.top

strlen(s)
来源：http://drw.sjlbkw.cn

[S06] C：字符串比较
来源：http://agf.sjlbkw.cn

strcmp(a, b) == 0
来源：http://jtn.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://iju.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uav.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://zrf.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qzp.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://rqw.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://amv.hcnkem.com

[S10] C：指针与解引用
来源：http://tww.jianghu66.top

int *p = &a;  *p = 5;
来源：http://fos.hammf.cn

[S11] C：逐行读文件
来源：http://gtw.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://wos.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nva.guannengcc.top

fclose(f);
来源：http://lte.ydzc1.top

[S12] C：写文件
来源：http://ijh.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vbs.sweek.top

[S13] C：宏定义
来源：http://tjw.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gsk.fktsv.cn

[S14] C：枚举
来源：http://lra.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://ojy.hesvh.cn

[S15] C：类型转换
来源：http://wjg.quarkkingdee.top

(double) a / b
来源：http://efe.zdbjq.cn

[S16] C：位操作置位
来源：http://bch.shangyingyoupin.top

x |= (1 << 3);
来源：http://sed.52xcode.cn

[S17] C：安全拼接字符串
来源：http://pbh.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://knp.dianchejie.cn

[S18] C：命令行参数
来源：http://aoq.daria6918.cn

int main(int argc, char **argv)
来源：http://sbg.zhixingplan.top

[S19] C：快速排序
来源：http://yee.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://pop.guannengcc.top

[S20] C：二分查找
来源：http://xal.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sfc.jinyuanbaomall.cn

[S21] C：字符类别判断
来源：http://ilp.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jjc.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://pbz.xziqi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mgq.hnqzz.top

[S23] C：随机数
来源：http://gvg.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rqc.snrcjt.cn

[S24] C：获取本地时间
来源：http://ycz.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kky.jiagoushi.top

[S25] C：内存拷贝
来源：http://egm.kuanghao11.cn

memcpy(dst, src, n);
来源：http://okm.hfpthk.cn

[S26] C：内存清零
来源：http://uni.fzhhl.top

memset(a, 0, sizeof a);
来源：http://wtx.sxryk.cn

[S27] C：定义常量
来源：http://aen.chenzaomai.com

const double PI = 3.14159;
来源：http://sry.sweek.top

[S28] C：静态变量
来源：http://fgk.shuidangran.top

static int counter = 0;
来源：http://jnz.yuanzhike.top

[S29] C：变参函数
来源：http://hpl.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cnd.jqgufenzy.top

[S30] C：头文件保护
来源：http://oes.tian-w.cn

#ifndef X_H
来源：http://pcm.yongpay.top

#define X_H
来源：http://xbn.xingfuxueyuan.xyz

#endif
来源：http://jjr.vehdjk.com

[S31] C++：Hello World
来源：http://bek.smart0.xyz

#include <iostream>
来源：http://xbn.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://jvt.gzhubu.top

[S32] C++：字符串
来源：http://rbp.yonumen.top

std::string s = "hi";  s += "!";
来源：http://yel.sweek.top

[S33] C++：vector 增删
来源：http://tvi.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ize.vehdjk.com

[S34] C++：遍历 vector
来源：http://mgx.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://ftv.cqqwz.cn

[S35] C++：map
来源：http://ecw.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://til.52xcode.cn

[S36] C++：unordered_map
来源：http://fwe.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aed.daxiang520.top

[S37] C++：set
来源：http://gjr.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fyd.yj20258888.top

[S38] C++：排序
来源：http://kye.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://ssn.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://uqc.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oec.cdnleiting.top

[S40] C++：查找元素
来源：http://iuc.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fmz.pycfn.com

[S41] C++：类与构造函数
来源：http://kfr.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lqu.fehbvm.com

[S42] C++：继承与虚函数
来源：http://usw.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://dkc.hesvh.cn

[S43] C++：智能指针
来源：http://xsn.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://snw.sxryk.cn

[S44] C++：引用传参
来源：http://mpp.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://pyt.fzhhl.top

[S45] C++：lambda
来源：http://dch.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://ybl.jiagoushi.top

[S46] C++：函数模板
来源：http://ucb.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://all.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://txk.haohaochexian.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jef.52xcode.cn

[S48] C++：逐行读文件
来源：http://znz.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://maj.andypj.xyz

while (std::getline(in, line)) { }
来源：http://lmb.chenzaomai.com

[S49] C++：写文件
来源：http://unx.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fcj.sweek.top

[S50] C++：格式化数字
来源：http://bjy.zhongyouzk.top


<!-- 参考信息 -->