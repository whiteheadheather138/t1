代发 wailian999

SHOW INDEX FROM users;
来源：http://cxo.gzhubu.top

[Q73] 查看表状态
来源：http://tge.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://yns.yj20258888.top

[Q74] 强制使用索引
来源：http://bhd.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zmg.ydzc1.top

[Q75] 日期格式化
来源：http://gmi.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://myj.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dns.tarul.cn

[Q76] 按天统计
来源：http://wdm.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sct.fanxiaobao.xyz

[Q77] 时间加减
来源：http://pgc.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://voi.shuidangran.top

[Q78] 当前时间
来源：http://mqk.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://htp.vehdjk.com

[Q79] 字符串拼接
来源：http://nuk.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hpj.mhx1999.top

[Q80] 字符串截取
来源：http://sos.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aqv.fktsv.cn

[Q81] 字符串替换
来源：http://btj.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bzl.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://uvo.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mek.wangshuangyany.cn

[Q83] 大小写转换
来源：http://mpo.fktsv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gcc.yonumen.top

[Q84] 去除首尾空格
来源：http://jpw.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://vkw.dianchejie.cn

[Q85] 数值取整
来源：http://uir.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dnn.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://mbz.xingfuxueyuan.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ivb.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://yfx.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kyq.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://mhf.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hla.bbcook.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nfb.hywenlv.cn

[Q89] 判断表是否存在
来源：http://hrm.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vhg.yonumen.top

[Q90] 生成序号列
来源：http://qpu.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmv.jinyuanbaomall.cn

================================================================================
来源：http://wxa.zhijiandao.cn

R. Bash 专题
来源：http://ixf.nanxuanxn.top

================================================================================
来源：http://vej.shuidangran.top

[R01] shebang 与严格模式
来源：http://dqn.aizwys.cn

#!/usr/bin/env bash
来源：http://cjl.xziqi.cn

set -euo pipefail
来源：http://ozf.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://dtf.ctjpmb.com

name="Tom"; echo "$name"
来源：http://uif.vehdjk.com

[R03] 只读变量
来源：http://cxl.daxiang520.top

readonly PI=3.14
来源：http://vct.fengsongda.top

[R04] 位置参数
来源：http://yei.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kfi.yj20258888.top

[R05] 参数默认值
来源：http://elw.52xcode.cn

name="${1:-default}"
来源：http://hlf.jiagoushi.top

[R06] 判断命令是否存在
来源：http://tns.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eme.hesvh.cn

[R07] if 判断文件
来源：http://zzn.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://soe.mhx1999.top

[R08] 数值比较
来源：http://byp.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vpf.yj202588.top

[R09] 字符串比较
来源：http://lca.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lus.ybcxt.top

[R10] 正则匹配
来源：http://nbb.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mdm.c1oappe.top

[R11] case 多分支
来源：http://ouh.snrcjt.cn

case "$1" in
来源：http://nae.cheryme.top

start) echo "启动" ;;
来源：http://kql.daxiang520.top

stop)  echo "停止" ;;
来源：http://ikv.sxryk.cn

*)     echo "未知命令" ;;
来源：http://sqp.hysaishi.cn

esac
来源：http://llw.yuanzhike.top

[R12] for 遍历文件
来源：http://wwk.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://sur.jinqigfzy.top

[R13] for 计数循环
来源：http://bjl.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://wae.yfazqb.com

[R14] C 风格 for
来源：http://sti.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lzz.cqqwz.cn

[R15] while 逐行读文件
来源：http://pmw.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://omn.cdnleiting.top

[R16] until 等待条件
来源：http://gmw.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qxr.sysykeji.top

[R17] 数组定义与取值
来源：http://zpa.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://lld.zhixingplan.top

[R18] 遍历数组
来源：http://wcc.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ota.gogol.net.cn

[R19] 数组长度
来源：http://ubc.tian-w.cn

echo "${#arr[@]}"
来源：http://fqe.ctjpmb.com

[R20] 关联数组（字典）
来源：http://hwy.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wsu.9152youxi.cn

[R21] 字符串长度
来源：http://dir.yangfankeji.com

echo "${#s}"
来源：http://riu.wangshuangyany.cn

[R22] 截取子串
来源：http://mkq.birdmap.top

echo "${s:0:5}"
来源：http://dkp.sxryk.cn

[R23] 字符串替换
来源：http://xbn.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kcv.nanxuanxn.top

[R24] 大小写转换
来源：http://muw.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hvr.xylfe.cn

[R25] 去后缀 / 去前缀
来源：http://fuc.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lcu.vehdjk.com

[R26] 命令替换
来源：http://ljw.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://njy.haohaochexian.top

[R27] 算术展开
来源：http://iuo.sysykeji.top

echo $((1 + 2 * 3))
来源：http://lwm.meibo888.top

[R28] 浮点运算
来源：http://ksw.daria6918.cn

echo "scale=2; 10/3" | bc
来源：http://aso.zdbjq.cn

[R29] 定义函数
来源：http://qai.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sfv.hcnkem.com

[R30] 函数返回状态码
来源：http://saa.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://vaa.yvedp.cn

[R31] 局部变量
来源：http://lpg.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://qsn.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://krf.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://syl.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://ter.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yia.52xcode.cn

[R34] 退出时清理
来源：http://jaz.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qjv.hysaishi.cn

[R35] 后台执行并等待
来源：http://mxk.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xlg.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://xls.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lff.yongpay.top

[R37] 把输出赋给变量
来源：http://whe.haohaochexian.top

files=$(ls -1)
来源：http://bim.haohaochexian.top

[R38] 管道串联
来源：http://teu.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://kuv.sweek.top

[R39] 重定向标准输出与错误
来源：http://eks.guowangkeji.top

cmd > out.log 2>&1
来源：http://nfx.ydjk.org.cn

[R40] 追加写日志
来源：http://dmv.zycfv.cn

echo "log" >> out.log
来源：http://agm.yj202588.top

[R41] 丢弃输出
来源：http://mpf.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://wsx.xylfe.cn

[R42] 输入重定向
来源：http://iin.wangshuangyany.cn

wc -l < a.txt
来源：http://xam.xylfe.cn

[R43] 按名字查找文件
来源：http://xfr.xuanzx.com

find . -name "*.log" -type f
来源：http://ekd.hysaishi.cn

[R44] 按修改时间查找
来源：http://yva.jiagoushi.top

find . -mtime -7 -type f
来源：http://jeo.tarul.cn

[R45] 批量删除
来源：http://keo.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://gdu.316326.xyz

[R46] 递归替换文件内容
来源：http://szd.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mma.hesvh.cn

[R47] sed 单行替换
来源：http://eke.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://jeu.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://lvw.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://tjo.hammf.cn

[R49] awk 带条件
来源：http://gvx.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ewm.sufxvd.cn

[R50] awk 求和
来源：http://xmk.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cfd.hysaishi.cn

[R51] 排序去重取前几
来源：http://fan.gzhubu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uzf.dashuyun.cn

[R52] 统计行数
来源：http://nfz.zhaomingkeji.xyz

wc -l a.txt
来源：http://ezi.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://lyv.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tkk.epnwcf.com

[R54] 比较两个文件
来源：http://pql.fanxiaobao.xyz

diff a.txt b.txt
来源：http://tpn.hywenlv.cn

[R55] 压缩与解压
来源：http://vof.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wgs.havefunace.top

[R56] 远程拷贝
来源：http://hrj.hfpthk.cn

scp file user@host:/path/
来源：http://fia.jyoumei.cn

[R57] 远程执行命令
来源：http://kss.nanxinkj.top

ssh user@host 'uptime'
来源：http://rpa.jqgfzy.top

[R58] 下载文件
来源：http://xha.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uye.nwbrower.top

[R59] 发 POST JSON
来源：http://rkf.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://okt.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://ltx.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gsu.ctjpmb.com

[R61] 磁盘占用
来源：http://awu.mhx1999.top

df -h;  du -sh *
来源：http://eva.sxryk.cn

[R62] 找最占空间的文件
来源：http://oke.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://yxm.hywenlv.cn

[R63] 内存与进程
来源：http://bkb.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://nno.chenzaomai.com

[R64] 结束进程
来源：http://ukp.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://gjz.chenzaomai.com

[R65] 查看端口占用
来源：http://ecf.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ajh.wangshuangyany.cn

[R66] 定时任务
来源：http://ram.guannengcc.top

crontab -e;  crontab -l
来源：http://emh.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://qsh.daxiang520.top

openssl rand -hex 16
来源：http://nch.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://bvg.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bxx.jianghu66.top

[R69] 生成随机密码
来源：http://fno.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://giy.haohaochexian.top

[R70] 时间戳与互转
来源：http://bee.52xcode.cn

date +%s;  date -d @1700000000
来源：http://yen.ctjpmb.com

[R71] 日期格式化
来源：http://uas.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kum.xylfe.cn

[R72] 等待端口就绪
来源：http://jdu.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://coh.tanke756.top

[R73] 分割大日志
来源：http://nck.iojbl.cn

split -l 1000 big.log part_
来源：http://jov.sysykeji.top

[R74] 批量重命名
来源：http://ule.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eur.cucudq.cn

[R75] 导出环境变量
来源：http://ddc.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://ndx.chenjidiqi.icu

[R76] 使用临时文件
来源：http://ehn.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tzq.yj20258.top

[R77] 读取用户输入
来源：http://yas.xinyue.icu

read -rp "请输入: " ans
来源：http://jjn.haohaochexian.top

[R78] 交互式菜单
来源：http://ckc.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zkn.yfazqb.com

[R79] 解析命令行选项
来源：http://vrm.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eta.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://din.vehdjk.com

time ./run.sh
来源：http://woj.tarul.cn

================================================================================
来源：http://rxm.ehwqpu.com

S. C / C++ 专题
来源：http://nsm.chenlongwang.top

================================================================================
来源：http://eat.aibaodan.cn

[S01] C：Hello World
来源：http://byq.haohaochexian.top

#include <stdio.h>
来源：http://gzs.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ipw.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://www.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://fyv.xylfe.cn

[S03] C：读入整数
来源：http://axe.zhengqikj.top

int x; scanf("%d", &x);
来源：http://oag.hnxiangtu.top

[S04] C：字符串复制
来源：http://ugb.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://ofv.shzxlz.cn

[S05] C：字符串长度
来源：http://fal.sweek.top

strlen(s)
来源：http://fxa.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://xzm.fzhhl.top

strcmp(a, b) == 0
来源：http://wjb.xziqi.cn

[S07] C：数组遍历求和
来源：http://izi.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://axt.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://bqn.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bjp.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://dxi.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://efh.kuanghao11.cn

[S10] C：指针与解引用
来源：http://sxi.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://pyz.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://qey.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://lzp.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ueg.daxiang520.top

fclose(f);
来源：http://uce.sxryk.cn

[S12] C：写文件
来源：http://eic.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ord.yuanzhike.top

[S13] C：宏定义
来源：http://qef.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mdl.fktsv.cn

[S14] C：枚举
来源：http://cju.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://wem.zycfv.cn

[S15] C：类型转换
来源：http://qtd.aizwys.cn

(double) a / b
来源：http://gxs.pycfn.com

[S16] C：位操作置位
来源：http://ohw.yj202588.top

x |= (1 << 3);
来源：http://bhe.hesvh.cn

[S17] C：安全拼接字符串
来源：http://nul.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://anz.9152youxi.cn

[S18] C：命令行参数
来源：http://ecc.cheryme.top

int main(int argc, char **argv)
来源：http://yfu.epnwcf.com

[S19] C：快速排序
来源：http://mwo.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://uwd.chenzaomai.com

[S20] C：二分查找
来源：http://kzq.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jca.hcnkem.com

[S21] C：字符类别判断
来源：http://htj.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pqk.yj20258888.top

[S22] C：字符串转数字
来源：http://pjt.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://bgk.xinyue.icu

[S23] C：随机数
来源：http://bqv.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://flp.jlsjyb.cn

[S24] C：获取本地时间
来源：http://sgo.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iin.zycfv.cn

[S25] C：内存拷贝
来源：http://doj.fktsv.cn

memcpy(dst, src, n);
来源：http://ztk.sxryk.cn

[S26] C：内存清零
来源：http://lcg.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://sjq.sufxvd.cn

[S27] C：定义常量
来源：http://cmx.jyoumei.cn

const double PI = 3.14159;
来源：http://nsn.xinyue.icu

[S28] C：静态变量
来源：http://mnb.sweek.top

static int counter = 0;
来源：http://pva.cqqwz.cn

[S29] C：变参函数
来源：http://sqd.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://soh.nanxinkj.top

[S30] C：头文件保护
来源：http://pwd.chenlongwang.top

#ifndef X_H
来源：http://pir.nanxuanxn.top

#define X_H
来源：http://fig.snrcjt.cn

#endif
来源：http://vpm.yonumen.top

[S31] C++：Hello World
来源：http://nay.tarul.cn

#include <iostream>
来源：http://cda.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://ity.ydjk.org.cn

[S32] C++：字符串
来源：http://dru.pycfn.com

std::string s = "hi";  s += "!";
来源：http://mbh.c1oappe.top

[S33] C++：vector 增删
来源：http://ddp.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ccm.jqgfzy.top

[S34] C++：遍历 vector
来源：http://emq.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://psw.bjfxy.top

[S35] C++：map
来源：http://rul.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rma.ydzc1.top

[S36] C++：unordered_map
来源：http://afz.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ray.zdbjq.cn

[S37] C++：set
来源：http://lis.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rhs.bbcook.cn

[S38] C++：排序
来源：http://adb.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://dbi.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://ucp.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zap.0kj1m.cn

[S40] C++：查找元素
来源：http://yvt.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://alv.pycfn.com

[S41] C++：类与构造函数
来源：http://ygy.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ggh.hcnkem.com

[S42] C++：继承与虚函数
来源：http://ulq.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://jkv.redwolf501.top


<!-- 参考信息 -->