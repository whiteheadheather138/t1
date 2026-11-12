代发 wailian999

ROLLBACK TO sp1;
来源：http://srn.hnxiangtu.top

[Q69] 查看执行计划
来源：http://zao.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lah.yuxming.cn

[Q70] 更新统计信息
来源：http://xyn.nanxuanxn.top

ANALYZE TABLE users;
来源：http://vmv.xingfuxueyuan.xyz

[Q71] 查看建表语句
来源：http://qrj.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hvf.guowangkeji.top

[Q72] 查看索引
来源：http://ppa.havefunace.top

SHOW INDEX FROM users;
来源：http://drm.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://ifr.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qxa.ydjk.org.cn

[Q74] 强制使用索引
来源：http://nno.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tfg.pengpengdd.cyou

[Q75] 日期格式化
来源：http://jjx.quarkkingdee.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lzb.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tfp.haohaochexian.top

[Q76] 按天统计
来源：http://zgv.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xyh.fanxiaobao.xyz

[Q77] 时间加减
来源：http://imn.shzxlz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://inr.tian-w.cn

[Q78] 当前时间
来源：http://isn.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dgg.c1oappe.top

[Q79] 字符串拼接
来源：http://nfy.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uyc.svipenyu.cn

[Q80] 字符串截取
来源：http://nen.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ejw.zdbjq.cn

[Q81] 字符串替换
来源：http://ovm.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wej.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://bae.xylfe.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uhi.pengpengdd.cyou

[Q83] 大小写转换
来源：http://vrf.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://twv.quarkkingdee.top

[Q84] 去除首尾空格
来源：http://uzd.pengpengdd.cyou

SELECT TRIM(name) FROM users;
来源：http://vuj.zhongyouzk.top

[Q85] 数值取整
来源：http://wpo.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vhd.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://pqr.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wfs.xylfe.cn

[Q87] JSON 字段做条件
来源：http://xov.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mep.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://bkb.hfpthk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dqp.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uvi.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://dwf.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oln.vehdjk.com

[Q90] 生成序号列
来源：http://csj.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jpi.cdnleiting.top

================================================================================
来源：http://fny.jyoumei.cn

R. Bash 专题
来源：http://xhr.jyoumei.cn

================================================================================
来源：http://bym.xziqi.cn

[R01] shebang 与严格模式
来源：http://ihx.yj20258888.top

#!/usr/bin/env bash
来源：http://agv.feifeiyinyue.top

set -euo pipefail
来源：http://klr.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://bnj.52xcode.cn

name="Tom"; echo "$name"
来源：http://hqm.hnqzz.top

[R03] 只读变量
来源：http://fyw.tanke756.top

readonly PI=3.14
来源：http://fie.xziqi.cn

[R04] 位置参数
来源：http://ihc.fengsongda.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://abo.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://bfy.yonumen.top

name="${1:-default}"
来源：http://whk.sweek.top

[R06] 判断命令是否存在
来源：http://usg.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yue.aizwys.cn

[R07] if 判断文件
来源：http://xcs.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://njq.jianghu66.top

[R08] 数值比较
来源：http://szz.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wfm.zhongyouzk.top

[R09] 字符串比较
来源：http://wvx.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dhi.shzxlz.cn

[R10] 正则匹配
来源：http://naz.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dtz.jinqigfzy.top

[R11] case 多分支
来源：http://fxo.epnwcf.com

case "$1" in
来源：http://mwb.cashguo.top

start) echo "启动" ;;
来源：http://bcx.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://rpw.guannengcc.top

*)     echo "未知命令" ;;
来源：http://djh.zdbjq.cn

esac
来源：http://fxl.bbcook.cn

[R12] for 遍历文件
来源：http://ryw.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://yxv.zhixingplan.top

[R13] for 计数循环
来源：http://xxs.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://nya.haohaochexian.top

[R14] C 风格 for
来源：http://kqr.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vli.quarkkingdee.top

[R15] while 逐行读文件
来源：http://ris.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cek.vehdjk.com

[R16] until 等待条件
来源：http://jdm.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qzg.yonumen.top

[R17] 数组定义与取值
来源：http://sux.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ojm.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://evb.yanxiufei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gyv.fanxiaobao.xyz

[R19] 数组长度
来源：http://twu.ctjpmb.com

echo "${#arr[@]}"
来源：http://ppm.yueranfly.top

[R20] 关联数组（字典）
来源：http://eeb.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tgo.xuetiantiany.cn

[R21] 字符串长度
来源：http://vbs.sweek.top

echo "${#s}"
来源：http://vac.tarul.cn

[R22] 截取子串
来源：http://qil.jyoumei.cn

echo "${s:0:5}"
来源：http://eme.gotoacloud.top

[R23] 字符串替换
来源：http://rst.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zep.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://bly.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://dlc.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://nhz.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pov.birdmap.top

[R26] 命令替换
来源：http://nti.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://iwa.daxiang520.top

[R27] 算术展开
来源：http://ajn.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://goy.andypj.xyz

[R28] 浮点运算
来源：http://uzs.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://wuj.aizwys.cn

[R29] 定义函数
来源：http://fhd.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hlf.guannengcc.top

[R30] 函数返回状态码
来源：http://viv.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://tjq.c1oappe.top

[R31] 局部变量
来源：http://ccr.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://bvh.ybcxt.top

[R32] 参数个数校验
来源：http://wef.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hqv.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://aip.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rqh.sjlbkw.cn

[R34] 退出时清理
来源：http://dwg.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rdu.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://ayo.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yej.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://aef.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ewj.hfpthk.cn

[R37] 把输出赋给变量
来源：http://nod.xziqi.cn

files=$(ls -1)
来源：http://xur.yuanzhike.top

[R38] 管道串联
来源：http://pmj.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://smn.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://nae.xinyue.icu

cmd > out.log 2>&1
来源：http://ecb.guannengcc.top

[R40] 追加写日志
来源：http://cob.yonumen.top

echo "log" >> out.log
来源：http://jjr.guannengcc.top

[R41] 丢弃输出
来源：http://bpv.andypj.xyz

cmd >/dev/null 2>&1
来源：http://sps.hcnkem.com

[R42] 输入重定向
来源：http://qfb.yj20258.top

wc -l < a.txt
来源：http://fjq.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://eiu.quarkkingdee.top

find . -name "*.log" -type f
来源：http://mqe.hfpthk.cn

[R44] 按修改时间查找
来源：http://lvh.yfazqb.com

find . -mtime -7 -type f
来源：http://yys.feifeiyinyue.top

[R45] 批量删除
来源：http://dkk.sysykeji.top

find . -name "*.tmp" -delete
来源：http://hua.birdmap.top

[R46] 递归替换文件内容
来源：http://ont.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://smd.meibo888.top

[R47] sed 单行替换
来源：http://vur.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://txp.sweek.top

[R48] awk 取指定列
来源：http://chz.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://zjv.gogol.net.cn

[R49] awk 带条件
来源：http://wgk.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ltw.epnwcf.com

[R50] awk 求和
来源：http://otb.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://een.zhixingplan.top

[R51] 排序去重取前几
来源：http://ine.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bfl.9152youxi.cn

[R52] 统计行数
来源：http://ynt.vqdsnc.cn

wc -l a.txt
来源：http://vmm.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://dkz.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rjk.fengsongda.top

[R54] 比较两个文件
来源：http://yqv.svipenyu.cn

diff a.txt b.txt
来源：http://ind.zycfv.cn

[R55] 压缩与解压
来源：http://jmk.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rmj.ehwqpu.com

[R56] 远程拷贝
来源：http://ciq.zhixingplan.top

scp file user@host:/path/
来源：http://xll.yonumen.top

[R57] 远程执行命令
来源：http://rfo.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://uhd.yj20258888.top

[R58] 下载文件
来源：http://pug.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hix.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://gun.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pnk.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://zzc.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fdt.sjlbkw.cn

[R61] 磁盘占用
来源：http://hta.bjfxy.top

df -h;  du -sh *
来源：http://jka.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://bqc.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://wcz.chenlongwang.top

[R63] 内存与进程
来源：http://syt.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://pwb.andypj.xyz

[R64] 结束进程
来源：http://wjp.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://pfq.dashuyun.cn

[R65] 查看端口占用
来源：http://dmo.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mdi.fanxiaobao.xyz

[R66] 定时任务
来源：http://bee.dashuyun.cn

crontab -e;  crontab -l
来源：http://yvv.yj20258.top

[R67] 生成随机十六进制串
来源：http://sts.gaohongyu789.top

openssl rand -hex 16
来源：http://tah.pycfn.com

[R68] 计算文件校验值
来源：http://nqs.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://jaf.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://dzi.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://ymk.dashuyun.cn

[R70] 时间戳与互转
来源：http://vpw.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://xij.quarkkingdee.top

[R71] 日期格式化
来源：http://fwr.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://olx.guowangkeji.top

[R72] 等待端口就绪
来源：http://lkl.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zga.hfpthk.cn

[R73] 分割大日志
来源：http://bte.ydzc1.top

split -l 1000 big.log part_
来源：http://zqa.zhengqikj.top

[R74] 批量重命名
来源：http://alj.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kra.yueranfly.top

[R75] 导出环境变量
来源：http://zfp.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://zam.sjlbkw.cn

[R76] 使用临时文件
来源：http://slc.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jyt.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://hpu.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://xns.andypj.xyz

[R78] 交互式菜单
来源：http://fkk.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xqt.jyoumei.cn

[R79] 解析命令行选项
来源：http://cix.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rza.yonumen.top

[R80] 查看脚本执行耗时
来源：http://ggp.jlsjyb.cn

time ./run.sh
来源：http://ley.nanxuanxn.top

================================================================================
来源：http://kir.zhongyouzk.top

S. C / C++ 专题
来源：http://wat.zdbjq.cn

================================================================================
来源：http://qoo.mhx1999.top

[S01] C：Hello World
来源：http://gpi.zhixingplan.top

#include <stdio.h>
来源：http://rwk.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qte.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://qov.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://vpu.kuanghao11.cn

[S03] C：读入整数
来源：http://tzc.tanke756.top

int x; scanf("%d", &x);
来源：http://ofj.shzxlz.cn

[S04] C：字符串复制
来源：http://fok.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://pjk.c1oappe.top

[S05] C：字符串长度
来源：http://sur.ybcxt.top

strlen(s)
来源：http://idx.hywenlv.cn

[S06] C：字符串比较
来源：http://flr.yj20258888.top

strcmp(a, b) == 0
来源：http://yoi.hcnkem.com

[S07] C：数组遍历求和
来源：http://rpm.ybcxt.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wsw.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://zco.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pjh.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://ksw.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yvk.guowangkeji.top

[S10] C：指针与解引用
来源：http://njo.aizwys.cn

int *p = &a;  *p = 5;
来源：http://bdb.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://kvk.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://tsp.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://acr.0kj1m.cn

fclose(f);
来源：http://upo.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://hkl.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ywu.yj20258.top

[S13] C：宏定义
来源：http://ogt.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vlf.jinqigfzy.top

[S14] C：枚举
来源：http://byg.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://jsw.zhongyouzk.top

[S15] C：类型转换
来源：http://hbc.cucudq.cn

(double) a / b
来源：http://mqh.mhx1999.top

[S16] C：位操作置位
来源：http://hyy.andypj.xyz

x |= (1 << 3);
来源：http://rct.guannengcc.top

[S17] C：安全拼接字符串
来源：http://pyu.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zmy.iojbl.cn

[S18] C：命令行参数
来源：http://eos.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://uvp.redwolf501.top

[S19] C：快速排序
来源：http://ejp.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://iwo.epnwcf.com

[S20] C：二分查找
来源：http://yne.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cgu.aibaodan.cn

[S21] C：字符类别判断
来源：http://yus.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ccq.yfazqb.com

[S22] C：字符串转数字
来源：http://zwu.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wco.tanke756.top

[S23] C：随机数
来源：http://uoo.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://esg.haohaochexian.top

[S24] C：获取本地时间
来源：http://zee.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tby.gaohongyu789.top

[S25] C：内存拷贝
来源：http://htq.jianghu66.top

memcpy(dst, src, n);
来源：http://xhl.cqqwz.cn

[S26] C：内存清零
来源：http://ijj.aizwys.cn

memset(a, 0, sizeof a);
来源：http://uvp.zycfv.cn

[S27] C：定义常量
来源：http://mfx.fehbvm.com

const double PI = 3.14159;
来源：http://fqu.dianchejie.cn

[S28] C：静态变量
来源：http://vmf.havefunace.top

static int counter = 0;
来源：http://caf.zhixingplan.top

[S29] C：变参函数
来源：http://qlv.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gpg.shangyingyoupin.top

[S30] C：头文件保护
来源：http://qju.gaohongyu789.top

#ifndef X_H
来源：http://gkv.hfpthk.cn

#define X_H
来源：http://iqu.pycfn.com

#endif
来源：http://mrj.hnqzz.top

[S31] C++：Hello World
来源：http://gjm.xylfe.cn

#include <iostream>
来源：http://urx.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://dot.tarul.cn

[S32] C++：字符串
来源：http://gfs.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://dzi.zhongyouzk.top

[S33] C++：vector 增删
来源：http://nnd.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bug.tian-w.cn

[S34] C++：遍历 vector
来源：http://opk.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://ntk.guannengcc.top

[S35] C++：map
来源：http://vma.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pyz.fehbvm.com

[S36] C++：unordered_map
来源：http://zfx.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://obf.andypj.xyz

[S37] C++：set
来源：http://jyq.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cwr.jqgufenzy.top

[S38] C++：排序
来源：http://gzq.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://mbc.gotoacloud.top


<!-- 参考信息 -->