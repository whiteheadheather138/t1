代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qvv.chenzaomai.com

[Q54] 清空表
来源：http://mni.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://loq.tian-w.cn

[Q55] 排名（并列占位）
来源：http://pld.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qtg.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://pea.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nuj.hcnkem.com

[Q57] 行号
来源：http://hvf.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zym.daxiang520.top

[Q58] 累计求和
来源：http://yoo.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qbt.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://hms.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pel.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://sjs.redwolf501.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wjd.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rkv.shzxlz.cn

[Q61] 移动平均
来源：http://vtz.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uyf.tanke756.top

[Q62] 分组占比
来源：http://itf.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ium.pycfn.com

[Q63] 开启事务
来源：http://qtl.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bul.shangyingyoupin.top

[Q64] 提交事务
来源：http://uic.yanxiufei.cn

COMMIT;
来源：http://ewr.shangyingyoupin.top

[Q65] 回滚事务
来源：http://zal.bjfxy.top

ROLLBACK;
来源：http://lyo.ppjwa.cn

[Q66] 行锁查询
来源：http://azy.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eyn.hnqzz.top

[Q67] 设置隔离级别
来源：http://oog.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pfo.fzhhl.top

[Q68] 保存点
来源：http://wav.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://xvb.svipenyu.cn

ROLLBACK TO sp1;
来源：http://ysm.dianchejie.cn

[Q69] 查看执行计划
来源：http://oyl.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yur.hnqzz.top

[Q70] 更新统计信息
来源：http://kga.aibaodan.cn

ANALYZE TABLE users;
来源：http://rzi.hysaishi.cn

[Q71] 查看建表语句
来源：http://eji.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bjb.quarkkingdee.top

[Q72] 查看索引
来源：http://pwg.fzhhl.top

SHOW INDEX FROM users;
来源：http://yku.jqgfzy.top

[Q73] 查看表状态
来源：http://dai.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rbq.nanxinkj.top

[Q74] 强制使用索引
来源：http://dyo.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dan.sweek.top

[Q75] 日期格式化
来源：http://lnh.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gdr.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vqz.zhengqikj.top

[Q76] 按天统计
来源：http://hou.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hnt.yonumen.top

[Q77] 时间加减
来源：http://dkk.bbcook.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lqc.ehwqpu.com

[Q78] 当前时间
来源：http://zfh.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tfn.jinqigfzy.top

[Q79] 字符串拼接
来源：http://flt.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mac.iojbl.cn

[Q80] 字符串截取
来源：http://pjw.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://voz.dashuyun.cn

[Q81] 字符串替换
来源：http://lem.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nkx.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://zhc.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mse.ybcxt.top

[Q83] 大小写转换
来源：http://ewc.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ozj.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://dtl.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://ybd.cdnleiting.top

[Q85] 数值取整
来源：http://rhx.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mtg.xinyue.icu

[Q86] 读取 JSON 字段
来源：http://rwp.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nqe.xinyue.icu

[Q87] JSON 字段做条件
来源：http://lvq.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fbq.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://zfl.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yfw.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kzw.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://skv.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uwj.jqgfzy.top

[Q90] 生成序号列
来源：http://kql.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://akq.svipenyu.cn

================================================================================
来源：http://dvu.zdbjq.cn

R. Bash 专题
来源：http://uey.fehbvm.com

================================================================================
来源：http://uyx.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://mrh.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://vrv.yvedp.cn

set -euo pipefail
来源：http://sft.sysykeji.top

[R02] 变量赋值与使用
来源：http://wom.ivvv.top

name="Tom"; echo "$name"
来源：http://lyw.ybcxt.top

[R03] 只读变量
来源：http://rik.shanyushiyangkeji.top

readonly PI=3.14
来源：http://xos.kuanghao11.cn

[R04] 位置参数
来源：http://xyo.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pjn.sweek.top

[R05] 参数默认值
来源：http://hjo.hesvh.cn

name="${1:-default}"
来源：http://djd.epnwcf.com

[R06] 判断命令是否存在
来源：http://gxv.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oip.zhijiandao.cn

[R07] if 判断文件
来源：http://ydx.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aac.dashuyun.cn

[R08] 数值比较
来源：http://tuj.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rlr.meibo888.top

[R09] 字符串比较
来源：http://kvk.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bfo.bjfxy.top

[R10] 正则匹配
来源：http://joj.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ywl.gogol.net.cn

[R11] case 多分支
来源：http://xkx.yueranfly.top

case "$1" in
来源：http://rka.xuetiantiany.cn

start) echo "启动" ;;
来源：http://lgw.xylfe.cn

stop)  echo "停止" ;;
来源：http://exv.bjfxy.top

*)     echo "未知命令" ;;
来源：http://xxr.uphjek.com

esac
来源：http://tua.tarul.cn

[R12] for 遍历文件
来源：http://jwa.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://mur.hammf.cn

[R13] for 计数循环
来源：http://tia.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://imb.zhoulong.xyz

[R14] C 风格 for
来源：http://sol.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lcb.yvedp.cn

[R15] while 逐行读文件
来源：http://nuy.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hmo.yuanzhike.top

[R16] until 等待条件
来源：http://pbv.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pri.zdqjudy.top

[R17] 数组定义与取值
来源：http://kln.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://dhp.yj202588.top

[R18] 遍历数组
来源：http://uct.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://unc.pengpengdd.cyou

[R19] 数组长度
来源：http://ffv.dianchejie.cn

echo "${#arr[@]}"
来源：http://zkj.meibo888.top

[R20] 关联数组（字典）
来源：http://smf.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zmb.yj20258888.top

[R21] 字符串长度
来源：http://szz.zhengqikj.top

echo "${#s}"
来源：http://bnr.gzhubu.top

[R22] 截取子串
来源：http://vfr.daria6918.cn

echo "${s:0:5}"
来源：http://epz.0kj1m.cn

[R23] 字符串替换
来源：http://onq.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dsz.hnxiangtu.top

[R24] 大小写转换
来源：http://bsj.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://hai.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://eud.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xuf.316326.xyz

[R26] 命令替换
来源：http://dan.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://uxn.yuanzhike.top

[R27] 算术展开
来源：http://ekm.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://xpw.fzhhl.top

[R28] 浮点运算
来源：http://jfs.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://ntl.yueranfly.top

[R29] 定义函数
来源：http://ryf.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vnf.kuanghao11.cn

[R30] 函数返回状态码
来源：http://kcm.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://aal.aibaodan.cn

[R31] 局部变量
来源：http://dai.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://lat.iojbl.cn

[R32] 参数个数校验
来源：http://jwy.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zvz.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://mci.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ebx.fzhhl.top

[R34] 退出时清理
来源：http://btt.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://smr.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://wkk.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dxn.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://czx.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ljm.jiagoushi.top

[R37] 把输出赋给变量
来源：http://ztz.smart0.xyz

files=$(ls -1)
来源：http://fjr.tianlin.xyz

[R38] 管道串联
来源：http://fbc.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://nki.aibaodan.cn

[R39] 重定向标准输出与错误
来源：http://rfb.ctjpmb.com

cmd > out.log 2>&1
来源：http://ujm.zhoulong.xyz

[R40] 追加写日志
来源：http://zhr.feifeiyinyue.top

echo "log" >> out.log
来源：http://nkn.vehdjk.com

[R41] 丢弃输出
来源：http://ohi.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://usz.shzxlz.cn

[R42] 输入重定向
来源：http://ihb.sjlbkw.cn

wc -l < a.txt
来源：http://joa.redwolf501.top

[R43] 按名字查找文件
来源：http://vfo.ctjpmb.com

find . -name "*.log" -type f
来源：http://hth.aibaodan.cn

[R44] 按修改时间查找
来源：http://pga.sjlbkw.cn

find . -mtime -7 -type f
来源：http://cil.chenzaomai.com

[R45] 批量删除
来源：http://iga.xziqi.cn

find . -name "*.tmp" -delete
来源：http://usz.ehwqpu.com

[R46] 递归替换文件内容
来源：http://vmw.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dkh.fktsv.cn

[R47] sed 单行替换
来源：http://cad.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://gst.52xcode.cn

[R48] awk 取指定列
来源：http://lod.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://izr.jinqigufen.top

[R49] awk 带条件
来源：http://qov.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ulx.zhiwuduotai.top

[R50] awk 求和
来源：http://pwv.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://ijt.316326.xyz

[R51] 排序去重取前几
来源：http://jdm.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xzn.daria6918.cn

[R52] 统计行数
来源：http://qlm.jinqigufen.top

wc -l a.txt
来源：http://sik.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://gtj.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bue.daxiang520.top

[R54] 比较两个文件
来源：http://zqm.fengsongda.top

diff a.txt b.txt
来源：http://wiq.zhoulong.xyz

[R55] 压缩与解压
来源：http://aib.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://njp.cashguo.top

[R56] 远程拷贝
来源：http://dfe.guannengcc.top

scp file user@host:/path/
来源：http://aon.tanke756.top

[R57] 远程执行命令
来源：http://fey.fengsongda.top

ssh user@host 'uptime'
来源：http://sxh.zdqjudy.top

[R58] 下载文件
来源：http://qnw.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gxo.jiagoushi.top

[R59] 发 POST JSON
来源：http://tan.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xlz.quarkkingdee.top

[R60] 只看 HTTP 状态码
来源：http://lqe.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zrz.guowangkeji.top

[R61] 磁盘占用
来源：http://dgu.gzhubu.top

df -h;  du -sh *
来源：http://yba.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://vmw.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://pgk.yongpay.top

[R63] 内存与进程
来源：http://tte.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://hcq.ydjk.org.cn

[R64] 结束进程
来源：http://rvx.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://qlg.yongpay.top

[R65] 查看端口占用
来源：http://lkk.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lep.guowangkeji.top

[R66] 定时任务
来源：http://sae.wangdashe.top

crontab -e;  crontab -l
来源：http://jve.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://ptu.shuidangran.top

openssl rand -hex 16
来源：http://kei.yueranfly.top

[R68] 计算文件校验值
来源：http://kkt.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://mbd.fktsv.cn

[R69] 生成随机密码
来源：http://gog.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://kxo.ehwqpu.com

[R70] 时间戳与互转
来源：http://onl.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://szi.gotoacloud.top

[R71] 日期格式化
来源：http://dly.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dox.jiagoushi.top

[R72] 等待端口就绪
来源：http://shj.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://arh.chenzaomai.com

[R73] 分割大日志
来源：http://cbu.yvedp.cn

split -l 1000 big.log part_
来源：http://nin.jlsjyb.cn

[R74] 批量重命名
来源：http://ksq.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ozs.52xcode.cn

[R75] 导出环境变量
来源：http://uif.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://ecz.shangyingyoupin.top

[R76] 使用临时文件
来源：http://xbb.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mdw.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://eyt.yfazqb.com

read -rp "请输入: " ans
来源：http://qbc.yueranfly.top

[R78] 交互式菜单
来源：http://tut.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://slq.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://jyj.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yaq.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://cnu.shangyingyoupin.top

time ./run.sh
来源：http://gyi.cheryme.top

================================================================================
来源：http://qvv.0kj1m.cn

S. C / C++ 专题
来源：http://sgb.zhixingplan.top

================================================================================
来源：http://zqr.hcnkem.com

[S01] C：Hello World
来源：http://ymw.shanyushiyangtech.top

#include <stdio.h>
来源：http://gfg.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://czm.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://cse.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://yng.epnwcf.com

[S03] C：读入整数
来源：http://pjq.zycfv.cn

int x; scanf("%d", &x);
来源：http://zvd.xuetiantiany.cn

[S04] C：字符串复制
来源：http://qwp.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mbz.yfazqb.com

[S05] C：字符串长度
来源：http://ovg.jianghu66.top

strlen(s)
来源：http://krt.zdqjudy.top

[S06] C：字符串比较
来源：http://ezv.fengsongda.top

strcmp(a, b) == 0
来源：http://xoo.sxryk.cn

[S07] C：数组遍历求和
来源：http://hjv.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oah.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://gqe.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wfk.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://mya.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fcz.dianchejie.cn

[S10] C：指针与解引用
来源：http://ook.cucudq.cn

int *p = &a;  *p = 5;
来源：http://sdc.52xcode.cn

[S11] C：逐行读文件
来源：http://rng.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://ymc.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sxi.xingfuxueyuan.xyz

fclose(f);
来源：http://ubv.kuanghao11.cn

[S12] C：写文件
来源：http://fzi.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pei.yvedp.cn

[S13] C：宏定义
来源：http://zvz.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hyd.jinghuilouyu.cn

[S14] C：枚举
来源：http://pld.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://dno.vqdsnc.cn

[S15] C：类型转换
来源：http://dkj.uphjek.com

(double) a / b
来源：http://nzb.pengpengdd.cyou

[S16] C：位操作置位
来源：http://esc.guowangkeji.top

x |= (1 << 3);
来源：http://gzb.cucudq.cn

[S17] C：安全拼接字符串
来源：http://zvj.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://egj.cheryme.top

[S18] C：命令行参数
来源：http://dis.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://ruf.xylfe.cn

[S19] C：快速排序
来源：http://hgn.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kti.hcnkem.com

[S20] C：二分查找
来源：http://oxx.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://taz.yongpay.top

[S21] C：字符类别判断
来源：http://gkf.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lru.gzhubu.top

[S22] C：字符串转数字
来源：http://idh.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://fel.andypj.xyz

[S23] C：随机数
来源：http://jco.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qhn.xinyue.icu

[S24] C：获取本地时间
来源：http://pvj.jyoumei.cn


<!-- 参考信息 -->