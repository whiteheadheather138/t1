代发 wailian999

[Q65] 回滚事务
来源：http://mvt.xuetiantiany.cn

ROLLBACK;
来源：http://okz.fengsongda.top

[Q66] 行锁查询
来源：http://xct.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qap.cqqwz.cn

[Q67] 设置隔离级别
来源：http://zdf.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gpt.ivvv.top

[Q68] 保存点
来源：http://gkm.cqqwz.cn

SAVEPOINT sp1;
来源：http://pug.cucudq.cn

ROLLBACK TO sp1;
来源：http://ogy.zycfv.cn

[Q69] 查看执行计划
来源：http://ymq.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://heu.zycfv.cn

[Q70] 更新统计信息
来源：http://rdy.tarul.cn

ANALYZE TABLE users;
来源：http://pdn.dianchejie.cn

[Q71] 查看建表语句
来源：http://nyl.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dfw.wangshuangyany.cn

[Q72] 查看索引
来源：http://zzd.ydzc1.top

SHOW INDEX FROM users;
来源：http://fsg.cqqwz.cn

[Q73] 查看表状态
来源：http://sjd.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://auu.gogol.net.cn

[Q74] 强制使用索引
来源：http://epv.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xhf.chenlongwang.top

[Q75] 日期格式化
来源：http://lnt.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qxa.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://byz.jiagoushi.top

[Q76] 按天统计
来源：http://hcr.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rfd.hongshengwenyu.top

[Q77] 时间加减
来源：http://nvi.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cfn.chenzaomai.com

[Q78] 当前时间
来源：http://qie.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sjp.gotoacloud.top

[Q79] 字符串拼接
来源：http://ugz.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vkc.dianchejie.cn

[Q80] 字符串截取
来源：http://dcd.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://myj.jlsjyb.cn

[Q81] 字符串替换
来源：http://zaj.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zeo.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://exz.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ssx.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://aci.52xcode.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://isf.chenzaomai.com

[Q84] 去除首尾空格
来源：http://piv.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://vpg.cashguo.top

[Q85] 数值取整
来源：http://mqo.birdmap.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xqr.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://swg.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://boz.fehbvm.com

[Q87] JSON 字段做条件
来源：http://rjt.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dhi.yonumen.top

[Q88] 行转列（条件聚合）
来源：http://cri.jianghu66.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eav.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jzu.zdqjudy.top

[Q89] 判断表是否存在
来源：http://kfn.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://myf.jinqigfzy.top

[Q90] 生成序号列
来源：http://viq.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lmk.iojbl.cn

================================================================================
来源：http://cyn.guowangkeji.top

R. Bash 专题
来源：http://xwo.0kj1m.cn

================================================================================
来源：http://cmg.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://cni.fzhhl.top

#!/usr/bin/env bash
来源：http://dpe.0kj1m.cn

set -euo pipefail
来源：http://tch.wangdashe.top

[R02] 变量赋值与使用
来源：http://shn.fktsv.cn

name="Tom"; echo "$name"
来源：http://wdf.316326.xyz

[R03] 只读变量
来源：http://kdg.sweek.top

readonly PI=3.14
来源：http://wrp.0kj1m.cn

[R04] 位置参数
来源：http://jjq.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mzd.chenlongwang.top

[R05] 参数默认值
来源：http://jok.sjlbkw.cn

name="${1:-default}"
来源：http://ipv.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://ypz.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kvi.xuetiantiany.cn

[R07] if 判断文件
来源：http://tbc.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aen.yj20258888.top

[R08] 数值比较
来源：http://gzo.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://nhl.hywenlv.cn

[R09] 字符串比较
来源：http://luy.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fun.jinqigufen.top

[R10] 正则匹配
来源：http://xcp.yj20258.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ffb.52xcode.cn

[R11] case 多分支
来源：http://eji.zhoulong.xyz

case "$1" in
来源：http://jyw.yfazqb.com

start) echo "启动" ;;
来源：http://tfs.shanyushiyangtech.top

stop)  echo "停止" ;;
来源：http://flp.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://gzx.svipenyu.cn

esac
来源：http://ppi.cdnleiting.top

[R12] for 遍历文件
来源：http://nrf.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://rau.zhiwuduotai.top

[R13] for 计数循环
来源：http://vrb.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://lhq.meibo888.top

[R14] C 风格 for
来源：http://zqc.zhixingplan.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ovs.bbcook.cn

[R15] while 逐行读文件
来源：http://hqk.shzxlz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cda.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://gjp.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://egw.yfazqb.com

[R17] 数组定义与取值
来源：http://dos.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://eva.9152youxi.cn

[R18] 遍历数组
来源：http://ftl.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rzo.xuetiantiany.cn

[R19] 数组长度
来源：http://iya.tanke756.top

echo "${#arr[@]}"
来源：http://uhc.haohaochexian.top

[R20] 关联数组（字典）
来源：http://ieu.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yaq.52xcode.cn

[R21] 字符串长度
来源：http://szh.fengsongda.top

echo "${#s}"
来源：http://jym.xuanzx.com

[R22] 截取子串
来源：http://vca.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://dmi.jqgfzy.top

[R23] 字符串替换
来源：http://nse.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://thu.zhixingplan.top

[R24] 大小写转换
来源：http://hnk.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://nuk.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://lfb.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://umw.sweek.top

[R26] 命令替换
来源：http://xys.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://lts.zycfv.cn

[R27] 算术展开
来源：http://cwa.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://hca.bjfxy.top

[R28] 浮点运算
来源：http://vba.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://ffz.zhoulong.xyz

[R29] 定义函数
来源：http://vhz.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://orv.tarul.cn

[R30] 函数返回状态码
来源：http://ene.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://evm.gaohongyu789.top

[R31] 局部变量
来源：http://ziu.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://czo.chenjidiqi.icu

[R32] 参数个数校验
来源：http://lsp.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kbo.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://rer.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wjc.chenjidiqi.icu

[R34] 退出时清理
来源：http://lsu.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://cfy.zdbjq.cn

[R35] 后台执行并等待
来源：http://ksi.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://irz.xylfe.cn

[R36] 并发执行多个任务
来源：http://hmu.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ufd.cucudq.cn

[R37] 把输出赋给变量
来源：http://axj.jiagoushi.top

files=$(ls -1)
来源：http://yqp.fehbvm.com

[R38] 管道串联
来源：http://mss.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://uxz.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://mxk.havefunace.top

cmd > out.log 2>&1
来源：http://xlu.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://krl.cucudq.cn

echo "log" >> out.log
来源：http://olo.hfpthk.cn

[R41] 丢弃输出
来源：http://vfv.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://rpg.bjfxy.top

[R42] 输入重定向
来源：http://hvs.vqdsnc.cn

wc -l < a.txt
来源：http://yhi.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://hoo.birdmap.top

find . -name "*.log" -type f
来源：http://edj.zhongyouzk.top

[R44] 按修改时间查找
来源：http://pgj.vqdsnc.cn

find . -mtime -7 -type f
来源：http://vir.yj202588.top

[R45] 批量删除
来源：http://zab.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://xrj.bbcook.cn

[R46] 递归替换文件内容
来源：http://bhq.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bdr.hnqzz.top

[R47] sed 单行替换
来源：http://bwl.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fss.cqqwz.cn

[R48] awk 取指定列
来源：http://zyp.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://gsf.bbcook.cn

[R49] awk 带条件
来源：http://pvg.yj202588.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zjh.havefunace.top

[R50] awk 求和
来源：http://rwv.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zgx.hnqzz.top

[R51] 排序去重取前几
来源：http://hyf.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oqg.wangshuangyany.cn

[R52] 统计行数
来源：http://ucl.shanyushiyangtech.top

wc -l a.txt
来源：http://uwa.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://mty.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bhk.9152youxi.cn

[R54] 比较两个文件
来源：http://sil.xinyue.icu

diff a.txt b.txt
来源：http://jpa.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://xcv.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kmj.epnwcf.com

[R56] 远程拷贝
来源：http://tyr.yfazqb.com

scp file user@host:/path/
来源：http://gau.hesvh.cn

[R57] 远程执行命令
来源：http://gld.fzhhl.top

ssh user@host 'uptime'
来源：http://ftm.zhengqikj.top

[R58] 下载文件
来源：http://tay.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zzg.jiagoushi.top

[R59] 发 POST JSON
来源：http://fqx.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://doj.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://hbt.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kak.yj20258888.top

[R61] 磁盘占用
来源：http://ceb.shanyushiyangtech.top

df -h;  du -sh *
来源：http://iso.fzhhl.top

[R62] 找最占空间的文件
来源：http://nbe.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://jey.shanyushiyangtech.top

[R63] 内存与进程
来源：http://ags.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://gex.yj202588.top

[R64] 结束进程
来源：http://nry.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://dgs.bbcook.cn

[R65] 查看端口占用
来源：http://aue.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fbf.gaohongyu789.top

[R66] 定时任务
来源：http://sqv.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://ush.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://xaz.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://pei.zdqjudy.top

[R68] 计算文件校验值
来源：http://qyg.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://qbu.hywenlv.cn

[R69] 生成随机密码
来源：http://faf.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://gtc.ctjpmb.com

[R70] 时间戳与互转
来源：http://eyj.yueranfly.top

date +%s;  date -d @1700000000
来源：http://ked.xylfe.cn

[R71] 日期格式化
来源：http://gfq.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kch.daria6918.cn

[R72] 等待端口就绪
来源：http://zlf.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://zut.hcnkem.com

[R73] 分割大日志
来源：http://qkk.dashuyun.cn

split -l 1000 big.log part_
来源：http://sce.yvedp.cn

[R74] 批量重命名
来源：http://tsu.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ewq.xylfe.cn

[R75] 导出环境变量
来源：http://das.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://mja.jqgufenzy.top

[R76] 使用临时文件
来源：http://opl.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ldx.fktsv.cn

[R77] 读取用户输入
来源：http://lny.hywenlv.cn

read -rp "请输入: " ans
来源：http://byn.jinqigufen.top

[R78] 交互式菜单
来源：http://qdb.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jgf.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://tvr.tanke756.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://icg.yj20258.top

[R80] 查看脚本执行耗时
来源：http://fgi.yj20258.top

time ./run.sh
来源：http://ecd.xuetiantiany.cn

================================================================================
来源：http://jnu.pengpengdd.cyou

S. C / C++ 专题
来源：http://uos.tarul.cn

================================================================================
来源：http://oyi.chenzaomai.com

[S01] C：Hello World
来源：http://wto.kuanghao11.cn

#include <stdio.h>
来源：http://oeb.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jpl.yj20258.top

[S02] C：变量与格式化输出
来源：http://stu.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://pbo.shanyushiyangtech.top

[S03] C：读入整数
来源：http://imw.ybcxt.top

int x; scanf("%d", &x);
来源：http://btx.hongshengwenyu.top

[S04] C：字符串复制
来源：http://zem.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://joo.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://tjn.9152youxi.cn

strlen(s)
来源：http://lni.sxryk.cn

[S06] C：字符串比较
来源：http://rpa.zhijiandao.cn

strcmp(a, b) == 0
来源：http://cnc.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://uob.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pjl.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://jza.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://urs.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://xla.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dgb.jqgufenzy.top

[S10] C：指针与解引用
来源：http://qek.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://zpm.snrcjt.cn

[S11] C：逐行读文件
来源：http://jxb.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://nqh.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nvg.vehdjk.com

fclose(f);
来源：http://gof.sufxvd.cn

[S12] C：写文件
来源：http://jqq.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vpv.zhixingplan.top

[S13] C：宏定义
来源：http://wjy.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ibr.yueranfly.top

[S14] C：枚举
来源：http://yxb.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://qxz.hfpthk.cn

[S15] C：类型转换
来源：http://duy.haohaochexian.top

(double) a / b
来源：http://gcm.ehwqpu.com

[S16] C：位操作置位
来源：http://yzj.hfpthk.cn

x |= (1 << 3);
来源：http://nwb.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://vak.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bhc.jiagoushi.top

[S18] C：命令行参数
来源：http://xmq.xylfe.cn

int main(int argc, char **argv)
来源：http://vee.hammf.cn

[S19] C：快速排序
来源：http://crq.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://lqa.shzxlz.cn

[S20] C：二分查找
来源：http://gqa.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vkl.jyoumei.cn

[S21] C：字符类别判断
来源：http://jtp.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bbx.hnxiangtu.top

[S22] C：字符串转数字
来源：http://ugc.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gxe.zhijiandao.cn

[S23] C：随机数
来源：http://ryt.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uno.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://xde.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rht.hesvh.cn

[S25] C：内存拷贝
来源：http://oxv.snrcjt.cn

memcpy(dst, src, n);
来源：http://twz.mhx1999.top

[S26] C：内存清零
来源：http://qjn.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://yye.chenlongwang.top

[S27] C：定义常量
来源：http://piv.wangdashe.top

const double PI = 3.14159;
来源：http://fjb.cashguo.top

[S28] C：静态变量
来源：http://tgr.xziqi.cn

static int counter = 0;
来源：http://xkc.guowangkeji.top

[S29] C：变参函数
来源：http://jfd.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mlg.guowangkeji.top

[S30] C：头文件保护
来源：http://pqt.gotoacloud.top

#ifndef X_H
来源：http://uma.sxryk.cn

#define X_H
来源：http://ayy.jlsjyb.cn

#endif
来源：http://tfr.hnxiangtu.top

[S31] C++：Hello World
来源：http://qtg.hesvh.cn

#include <iostream>
来源：http://tla.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://udf.ivvv.top

[S32] C++：字符串
来源：http://jxs.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://iaq.sweek.top

[S33] C++：vector 增删
来源：http://gbj.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wgv.tanke756.top

[S34] C++：遍历 vector
来源：http://eeg.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://eos.chenzaomai.com


<!-- 参考信息 -->